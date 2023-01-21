<script>
export default {
    data () {
        return {
            items: [
                {
                    text: 'Digital Comics',
                    img: 'buy-comics-digital-comics.png' 
                },
                {
                    text: 'DC Merchandise',
                    img: 'buy-comics-merchandise.png' 
                },
                {
                    text: 'Subscription',
                    img: 'buy-comics-subscriptions.png' 
                },
                {
                    text: 'Comic Shop locator',
                    img: 'buy-comics-shop-locator.png' 
                },
                {
                    text: 'Dc Power Visa',
                    img: 'buy-dc-power-visa.svg' 
                }
            ]
            
        }
    },

    methods: {
        buildImagePath (img) {
            const url = new URL(`../assets/img/${img}`, import.meta.url);
            return (url.href);
        }
    }
}

</script>



<template>
    <section>
        <ul>
            <li v-for="item in items">
                <img href="#" :src="buildImagePath(item.img)" alt="">
                <span> <a href="#"> {{ item.text }}</a> </span>
            </li>
        </ul>
    </section>

</template>



<style lang="scss" scoped>
    section {
        position: relative;
        z-index: 1;
        height: 250px;
        background-color: dodgerblue;
        display: flex;
        align-items: center;
        justify-content: center;
        ul {
            display: flex;
            align-items: center;

            li {
                text-transform: uppercase;
                display: flex;
                align-items: center;
                padding: 0 25px;

                a {
                    text-decoration: none;
                    color: white;
                }

                a:hover {
                    color: blanchedalmond;
                }
            }

        }
    }

    img {
        cursor: pointer;
        height: 75px;
        padding-right: 10px;
    }

</style>