<script>
export default {
    data () {
        return {
            DcComics: [

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
            ],

            Terms : ['Terms of use', 'Privacy policy', 'Ad choices', 'Advertising', 'Jobs', 'Subs', 'Talent Workshop', 'Cpsc certificates', 'Ratings', 'Shop help', 'Contact us'],

            Sites : ['DC', 'MAD magazine', 'DC kids', 'DC universe', 'DC Power Visa']
        }
    }
}
</script>




<template>
    <footer>
        <div class="container">

            <nav>
            <!-- lista di Dc comics  -->
                <div class="dc-comics">
                    <ul>
                        <h2>
                            DC COMICS
                        </h2>
                        <li v-for="DcComic in DcComics">
                            <a href="">{{ DcComic.text }} </a>
                        </li>
                    </ul>
            
                    <ul>
                        <h2>
                            SHOP
                        </h2>
                        <li>
                            <a href="#"> Shop dc  </a>
                        </li>
                        <li>
                            <a href="#"> Shop dc Collectibles </a>
                        </li>
                    </ul>
                </div>
    
                <div class="dc-terms">
                    <ul>
                        <h2>
                            DC
                        </h2>
                        <li v-for="Term in Terms">
                            <a href="#"> {{ Term }} </a>
                        </li>
                    </ul>
                </div>
    
                <div class="sites">
                    <ul>
                        <h2>
                            SITES
                        </h2>
                        <li v-for="Site in Sites">
                            <a href="#"> {{ Site }} </a>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
    </footer>
</template>



<style lang="scss" scoped>
    footer {
        height: calc(100vh - 350px);
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;

    }

    nav {
        display: flex;
        width: 50%;
        padding: 4rem 0;

            * {   
                flex-basis: calc(100% / 3)
            }
    }


    ul {

        h2 {
            color: white;
        }
        li a {
            color: gray;
        }
    }
</style>        