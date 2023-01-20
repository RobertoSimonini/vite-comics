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

            <figure>
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </figure>
        </div>

            <div id="footer-bottom">
                <!-- Parte sinistra del footer-bottom con bottone di accedi  -->
                <div class="sign-up">
                    <button >
                        SIGN-UP NOW!
                    </button>
                </div>

                <!-- Qui metto la parte destra del footer ove posso trovare i link dei social  -->
                <div class="social-medias">
                    <h2>
                        FOLLOW US
                    </h2>

                    <!-- QUi metto tutti i social  -->
                    <ul>
                        <li>
                            <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                        </li>

                        <li>
                            <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                        </li>

                        <li>
                            <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
                        </li>

                        <li>
                            <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                        </li>

                        <li>
                            <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
                        </li>
                        
                    </ul>
                </div>

            </div>

    </footer>
</template>



<style lang="scss" scoped>
    footer {
        height: 600px;
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

            ul {
                padding: 1rem 0;
                h2 {
                    color: white;
                    padding: 0;
                }
                li a {
                    color: gray;
                    line-height: 25px;
                }

                li a:hover {
                    color: white;
                    line-height: 25px;
                }
            }
    }


    #footer-bottom {
        padding: 0 12.5%;
        height: 150px;
        background-color: #303030;
        display: flex;
        align-items: center;
        justify-content: space-between;

        button {
            border: 1px solid dodgerblue;
            background-color: transparent;
            color: white;
            padding: 10px 20px;
            cursor: pointer;
            font-size: 18px;
        }
    }

    .social-medias {
        color: dodgerblue;
        display: flex;
        align-items: center;
        ul {
            display: flex;
           
        }

        ul > * {
            margin: 0 0.5rem;
        }
    }

    h2 {
        margin: 0;
        padding: 0 0.5rem;
    }

   
</style>        