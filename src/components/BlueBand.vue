<script>
export default {
    name: 'AppMain',
        data() {
            bluebarList: [
                {
                    image: 'buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    image: 'buy-comics-subscription-png',
                    text: 'SUBSCRIPTION'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    text: ' COMICS SHOP LOCATOR'
                },
                {
                    image: 'buy-dc-power-visa.png',
                    text: 'DC POWER VISA'
                }
            ]
        }
    }
</script>


<template>
    <section class="banner">
        <div class="my_container">
            <div class="banner-element" v-for="bannerElement in bluebarList">
                <img src="../assets/img/buy-comics-merchandise.png" :alt="bannerElement.text + '\'s image'">

            </div>

        </div>

    </section>

</template>

<style lang="scss">
@use '../styles/partials/variables' as *;

.my_container {
    display: flex;
    height: 8.5rem;
}

section.banner {
    background-color: $main-color;
    color: white;

    div.banner-element {
        display: flex;
        align-items: center;
        margin-right: 2rem;
    }
}

.flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.list {
    padding-top: 3rem;
}

img {
    height: 60px;
}

span {
    text-transform: uppercase;
    padding-left: 0.5rem;
}
</style>