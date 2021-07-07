<template>
    <section>
        <div class="container">
            <ProductsBox
            v-for="(prodotti,index) in arrayDc" 
            :key="index"
            :card="prodotti"/>
        </div>
        <div class="container-button">
            <button class="bianco uppercase">load more</button>
        </div>
    </section>
   
</template>

<script>
import ProductsDc from '@/data/ProductsDc.js'
import ProductsBox from '@/components/ProductsBox.vue'
export default {

    name:'SectionImg',
    components : {
        ProductsBox
    },
    data(){
        return{
            arrayDc : ProductsDc
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/flex.scss';
    @import '../style/button.scss';
    @import '../style/commons.scss';
    @import '../style/commons-font.scss';
    section {
        padding: 20px 0;
        background: #1c1c1c;

        .container {
            @include my-flex;
            flex-wrap: wrap;
            width: 100%

        }
        .container-button {
            @include flex-center;
            margin-top: 20px;
            button {
                @include button1(#0282f9,0,#0282f9,30px);
                font-size: 12px;
            }
        }

    }

    

</style>