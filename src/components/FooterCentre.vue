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
                        <li><a href="#"></a></li>
                        <li><a href="#"></a></li>
                    </ul>
                </div>
                

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
    footer {
        background-image: url('../assets/img/footer-bg.jpg');
        // height: 500px;
        background-size: cover;
        .container.footer-centre {
            display: flex;

            .box-liste {
                width: 50%;
                ul {
                    list-style: none;
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