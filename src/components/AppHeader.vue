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
    }
}
</script>

<template>
    <div class="container">
        <header>
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <nav>
                <ul>
                    <li v-for="link in links">
                         <a href="#"> {{ link.text }} </a> 
                    </li>
                </ul>
            </nav>
        </header>
    </div>
</template>


<style lang="scss" scoped>
    header {
        height: 150px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        ul {
            display: flex;
            li {
                margin: 0 1rem;
            }
        }
    }

    ul li a:hover {
        color: dodgerblue;
    }

</style>