<script>
export default {
    data () {
        return {
          links :  [
            {
                text: 'Characters',
                url: '#',
                current: false,
            },
            {
                text: 'Comics',
                url: '#',
                current: true,
            },
            {
                text: 'Movies',
                url: '#',
                current: false,
            },
            {
                text: 'TV',
                url: '#',
                current: false,
            },
            {
                text: 'Games',
                url: '#',
                current: false,
            },
            {
                text: 'Collectibles',
                url: '#',
                current: false,
            },
            {
                text: 'Videos',
                url: '#',
                current: false,
            },
            {
                text: 'Fans',
                url: '#',
                current: false,
            },
            {
                text: 'News',
                url: '#',
                current: false,
            },
            {
                text: 'Shop',
                url: '#',
                current: false,
            },
            ]
        }
    },

    methods: {
        changeActive(i){
            this.links[i].current = !this.links[i].current
        }
    }
}
</script>

<template>
    
        <header>
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <nav>
                <ul>
                    <li v-for="(link, i) in links" :class="{active: link.current}">
                         <a href="#" @click="changeActive(i)"> {{ link.text }} </a> 
                    </li>
                </ul>
            </nav>
        </header>
    
</template>


<style lang="scss" scoped>
    header {
        padding: 0 12.5%;
        height: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {
            height: 75px;
        }

        ul {
            display: flex;
            li {
                margin: 0 1rem;
                a {
                    font-size: 12.5px;
                    text-transform: uppercase;
                    color: black;
                }
            }
        }
    }

    ul li a:hover {
        color: dodgerblue;
    }

    .active {
        text-decoration: underline dodgerblue;
        color: dodgerblue;
    }

</style>