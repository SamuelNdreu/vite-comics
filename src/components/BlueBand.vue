<script>
export default {
        name: 'AppMain',
        data() {
            return {
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
        },
    methods: {
        getImagePath: fuction (imgPath) {
            return new URL (`../assets/img/${imgPath}`, import.meta.url).href;
        }

    }
}

</script>


<template>
    <section class="banner">
        <div class="my_container">
            <div class="banner-element" v-for="bannerElement in bluebarList">
                <img :src="getImagePath(bannerElement)" :alt="bannerElement.text + '\'s image'">
                <h4>Merchandise</h4>
            </div>

        </div>

    </section>

</template>

<style lang="scss">
@use '../styles/partials/variables' as *;

.my_container {
    display: flex;
    height: 10rem;
    justify-content: center;
    align-items: center;
}

section.banner {
    background-color: $main-color;
    
    div.banner-element{
        img{
            height: 65px;
            margin-right: 1rem;
        }
        display: flex;
        align-items: center;
        margin-left: 2rem;
        margin-right: 2rem;
        color: white;

    }
}

.flex {
    display: flex;
}

.list {
    padding-top: 3rem;
}



span {
    text-transform: uppercase;
    padding-left: 0.5rem;
}
</style>