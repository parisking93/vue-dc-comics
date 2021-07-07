<template>
    <div class="jumbo">
        <div class="container">
            <button class="bianco uppercase btn">current series</button>
        </div>
    </div>
</template>

<script>
export default {
    name : 'Jumbotron'
}
</script>

<style lang="scss" scoped>
    @import '../style/button.scss';
    @import '../style/commons.scss';
    @import '../style/commons-font.scss';

    .jumbo {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;

        .container {
            position: relative;
            height: 300px;
            
            .btn {
                position: absolute;
                top: calc(100% - 20px);
                left: 0px;
                font-size:18px;
                font-weight: bold;
                @include button1(#0282f9,0)
            }
        }  
    } 



</style>