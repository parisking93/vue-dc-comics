<template>
    <footer>
        <div class="container footer-up">
            <div class="box-icon" v-for="(icons,index) in icon" :key="index">
                <img :class="(icon.length - 1 == index) ? 'ultima-img':'' " :src="icons.adress" :alt="icons.name">
                <span class="bianco">{{icons.name.toUpperCase()}}</span>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name : 'FooterUp',
    data() {
        return {
            icon : [
                {
                    adress : require("@/assets/img/buy-comics-digital-comics.png"),
                    name : 'digital comics'
                },
                {
                    adress : require("@/assets/img/buy-comics-merchandise.png"),
                    name : 'dc merchadise'
                },
                {
                    adress : require("@/assets/img/buy-comics-shop-locator.png"),
                    name : 'comic shop locator'
                },
                {
                    adress : require("@/assets/img/buy-comics-subscriptions.png"),
                    name : 'subscription'
                },
                {
                    adress : require("@/assets/img/buy-dc-power-visa.svg"),
                    name : 'dc power visa'
                }
            ]
        }
        
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/commons.scss';
    @import '../style/commons-font.scss';
    @import '../style/flex.scss';


    footer {
        background: #0282f9;
    }
    .container.footer-up {
        @include my-flex;
        height: 140px;
        align-items: center;
        padding: 40px;
    }
    .box-icon {
        height: $maxHeight;
        text-align: center;
        cursor: pointer;
        img {
            height: $maxHeight;
            vertical-align: middle;
        }
        .ultima-img {
            width: 60px;
        }
        span {
            font-size: $fontSmall;
            margin-left: 10px;
        }


    }

</style>