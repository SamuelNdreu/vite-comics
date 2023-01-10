<script>
export default {
    name: 'AppMain',
    data () {
        bluebarList: [
            {
                image: 'buy-comics-digital-comics.png',
                text:  'DIGITAL COMICS'
            },
            {
                image: 'buy-comics-merchandise.png',
                text:  'DC MERCHANDISE'
            },
            {
                image: 'buy-comics-subscription-png',
                text:  'SUBSCRIPTION'
            },
            {
                image: 'buy-comics-shop-locator.png',
                text:  ' COMICS SHOP LOCATOR'
            },
            {
                image:'buy-dc-power-visa.png',
                text: 'DC POWER VISA'
            }
        ]
    }
}
</script>

<template>
    <div class="wrapper-top">
        <div class="container">
            <h1>Content goes here</h1>
        </div>
        <div class="wrapper-bottom">
            <div class="my_container">

            </div>

        </div>
    </div>    
</template>


    

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
    
    .my_container{
        display: flex;
        height: 10rem;
    }
    .wrapper-top{
        width: 100%;
        height: 110px;
        background-color: $main-dark-bg;
    }
     h1 {
        display: flex;
        align-items: center;
        color: rgb(235, 16, 16);
    }

</style>
