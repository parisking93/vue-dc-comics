<template>
  <footer>
        <div class="container footer-centre">
            <div class="box-liste bianco">
                <div class="box-liste-sinistra">
                    <ul>
                        <li class="uppercase"><h3>dc comics</h3></li>
                        <li><a href="#">caracters</a></li>
                        <li><a href="#">comics</a></li>
                        <li><a href="#">movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">games</a></li>
                        <li><a href="#">videos</a></li>
                        <li><a href="#">news</a></li>
                    </ul>
                    <ul>
                        <li><h3 class="uppercase">shop</h3></li>
                        <li><a href="#">shop dc</a></li>
                        <li><a href="#">shop dc collectibles</a></li>
                    </ul>
                </div>
                <ul>
                    <li><h3 class="uppercase">dc</h3></li>
                    <li><a href="#">terms of use</a></li>
                    <li><a href="#">privacy policy(new)</a></li>
                    <li><a href="#">ad choices</a></li>
                    <li><a href="#">advertising</a></li>
                    <li><a href="#">jobs</a></li>
                    <li><a href="#">subscritions</a></li>
                    <li><a href="#">talent workshop</a></li>
                    <li><a href="#">CPSC certificates</a></li>
                    <li><a href="#">ratings</a></li>
                    <li><a href="#">shop help</a></li>
                    <li><a href="#">contact us</a></li>
                </ul>
                <ul>
                    <li><h3 class="uppercase">sites</h3></li>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD  magazine</a></li>
                    <li><a href="#">DC  kids</a></li>
                    <li><a href="#">DC universe</a></li>
                    <li><a href="#">DC power visa</a></li>
                </ul>
                

            </div>
            <div class="box-img-dc">

            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name : "FooterCentre"
}
</script>

<style lang="scss" scoped>
    @import '../style/commons.scss';
    @import '../style/commons-font.scss';
    @import '../style/flex.scss';
    footer {
        background-image: url('../assets/img/footer-bg.jpg');
        // height: 500px;
        background-size: cover;
        .container.footer-centre {
            @include my-flex;

            .box-liste {
                @include my-flex;
                width: 30%;
                padding: 50px 0;

                ul {
                    list-style: none;
                    margin: 30px 0;
                    li {
                        a {
                            text-decoration: none;
                            color: $grey;
                            font-size: $fontSmall;
                            text-transform: capitalize;
                        }
                    }
                }
            }
            .box-img-dc {
                width: 50%;
                background-image: url('../assets/img/dc-logo-bg.png');
                background-size: cover;
                background-position: center;
            }


        }
    }

</style>