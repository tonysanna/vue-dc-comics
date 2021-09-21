<template>
    <footer>
        <div class="footer-top">
            <div class="container-t">
                <div class="container-sx-t">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>

                    <h3>DC</h3>
                    <ul>
                        <li>Term Of Use</li>
                        <li>Privacy</li>
                        <li>AS Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPsc Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>

                    <h3>SITES</h3>
                    <ul>
                        <li>DC</li>
                        <li>Mad Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power visa</li>
                    </ul>
                </div>
                <div class="col-dx-t">
                    <img src="../assets/img/dc-logo-bg.png" alt="DC logo grande">
                </div>
            </div>
        </div>
        <div class="footer b">
            <div class="container-b">
                <div class="col-sx-b">
                    <button>SIGN-UP NOW!</button>
                </div>

                <div class="col-dx-b">
                    <h3>FOLLOW US</h3>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>

export default {
    name:'Footer'
}
</script>

<style scoped lang="scss">
@import "../style/mood";

.footer-top {
    height: 400px;
    width: 100%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-position: top;

    .container-t {
        display: flex;
        justify-content: space-between;
        width: 70%;
        height: 100%;
        margin: 0 auto;

        .col-sx-t {
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            height: 100%;
            width: 40%;
            padding: 25px 0;

            h3 {
                color: $light;
                margin: 18px 0;
            }

            li {
                font-size: 12px;
                color: rgb(116, 113, 113);
                width: 150px;
                margin: 4px 0;
            }
        }
        
        .col-dx-t {
            width: 595px;

            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
            }
        }
    }
}

.footer-bott {
    width: 100%;
    height: 110px;
    background-color: #464545;

    .container-b {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        width: 70%;
        margin: 0 auto;

        .col-sx-b button {
            width: 130px;
            height: 50px;
            background-color: #464545;
            border: 3px solid $primary;
            color: honeydew;
            font-size: 15px;

        }
        

        .col-dx-b {
            display: flex;
            align-items: center;

            img {
                margin: 0 8px;
            }

            h3 {
                color: $primary;
                margin-left: 18px;
            }
        }
    }
}


</style>
