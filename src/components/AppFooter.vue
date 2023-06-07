<script>

export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>
        <div id="fcontainer">
            <div id="listfooter">
                <div>
                    <ul>
                        <li>
                            <h2>DC COMICS</h2>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <ul>
                        <li>
                            <h2>SHOP</h2>
                        </li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <ul>
                    <li>
                        <h2>DC</h2>
                    </li>
                    <li>Term of Use</li>
                    <li>Privacy policy (New)</li>
                    <li>Add Choices</li>
                    <li>advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certificates</li>
                    <li>Rating</li>
                    <li>Shop Help</li>
                    <li>Contact us</li>
                </ul>
                <ul>
                    <li>
                        <h2>SITES</h2>
                    </li>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power VISA</li>
                </ul>
            </div>
            <div id="megalogo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
        <div id="bottombar">
            <button>SIGN UP NOW!</button>
            <div id="boxsocial">
                <h3>FOLLOW US</h3>
                <div id="social">
                    <div class="contacts">
                        <img src="../assets/img/footer-facebook.png" alt="">
                    </div>
                    <div class="contacts">
                        <img src="../assets/img/footer-twitter.png" alt="">
                    </div>
                    <div class="contacts">
                        <img src="../assets/img/footer-youtube.png" alt="">
                    </div>
                    <div class="contacts">
                        <img src="../assets/img/footer-pinterest.png" alt="">
                    </div>
                    <div class="contacts">
                        <img src="../assets/img/footer-periscope.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

#fcontainer {
    @include my-display-flex-1;
    height: 270px;
    background-image: url('../assets/img/footer-bg.jpg');
    padding: 0 20%;

    #listfooter {
        width: 40%;
        display: flex;
        padding-top: 10px;

        ul {
            margin-inline: 15px;

            li {
                font-size: 10px;
                margin-block: 5px;
            }
        }
    }

    #megalogo {
        position: relative;
        top: -40px;
        width: 350px;
    }
}

#bottombar {
    height: 90px;
    background-color: $secondary-color;
    position: relative;
    z-index: 100000;
    align-items: center;
    @include my-display-flex-1;
    padding: 0 19%;


    button {
        background-color: $secondary-color;
        border: 2px solid $primary-color;
        padding: 10px;
        font-size: 18px;
        color: white;
    }

    #boxsocial {
        display: flex;
        align-items: center;
        color: $primary-color;

        #social {
            display: flex;
            margin-left: 20px;

            .contacts {
                width: 35px;
                margin-inline: 5px;
            }
        }


    }
}

img {
    width: 100%;
}
</style>