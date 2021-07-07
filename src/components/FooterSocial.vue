<template>
    <footer>
        <div class="container">
            <button class="uppercase bianco">sign-up now!!</button>
            <div class="container-icon">
                <span class="uppercase">follow us</span>
                <div class="container-awesome">
                    <i class="fab fa-facebook-f"></i>
                </div>
                <div class="container-awesome">
                    <i class="fab fa-twitter"></i>
                </div>
                 <div class="container-awesome">
                    <i class="fab fa-youtube"></i>
                </div>
                 <div class="container-awesome">
                    <i class="fab fa-pinterest-p"></i>
                </div>
                 <div class="container-awesome">
                    <i class="fas fa-map-marker-alt"></i>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>

export default {
    name : 'FooterSocial'
}
</script>

<style lang="scss" scoped>
    @import '../style/flex.scss';
    @import '../style/button.scss';
    @import '../style/commons.scss';
    @import '../style/commons-font.scss';



    footer {
        background-color: $grigioScuro;
        .container {
            @include my-flex;
            height: 90px;
            align-items: center;
            button {
                @include button1($grigioScuro,2px,$blu)
            }
            .container-icon {
                display: flex;
                align-items: center;
                height: $maxHeight;
                span {
                    color: $blu;
                    margin: 10px;
                }
                .container-awesome {
                    width: 30px;
                    height: 30px;
                    @include flex-center;
                    background-color: rgba(255,255,255,0.4);
                    border-radius: 50%;
                    margin: 5px;
                    cursor: pointer;
                }
            }
        }

    }

</style>