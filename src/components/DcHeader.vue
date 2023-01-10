<script>
export default {
    data() {
        return {
            menuItems: [
                {
                    text: 'Characters',
                    active: false
                },
                {
                    text: 'Comics',
                    active: true
                },
                {
                    text: 'Movies',
                    active: false
                },
                {
                    text: 'Tv',
                    active: false
                },
                {
                    text: 'Games',
                    active: false
                },
                {
                    text: 'Collectibles',
                    active: false
                },
                {
                    text: 'Videos',
                    active: false
                },
                {
                    text: 'Fans',
                    active: false
                },
                {
                    text: 'News',
                    active: false
                },
                {
                    text: 'Shop',
                    active: false
                },
            ]
        }
    },
}
</script>

<template>
    <div class="container">
        <div class="container">
            <div class="img-wrapper-logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav>
                <ul>
                    <li v-for="menuItem in menuItems" :class="(menuItem.active) ? 'active' : ''"> {{ menuItem.text }}
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.wrapper {
    width: 100%;
    height: 100%;
}

.img-wrapper-logo img {
    width: 80px;
}

nav ul {
    display: flex;
    list-style-type: none;
}

ul li {
    padding: 2.3rem .5rem;
    text-transform: uppercase;
    font-size: 1rem;
    font-weight: 700;
    
    &.active{
        border-bottom: 5px solid $main-color;
    }
}
</style>
