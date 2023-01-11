<script>
export default {
    props: [
        'thumbnail',
        'price',
        'series',
        'type'
    ],
}
</script>

<template>
    <div class>
        <div class="img-wrapper">
            <img :src="thumbnail">
            <h2>{{ series }}</h2>
             <p>{{ price }}</p>

        </div>
    </div>
</template>

<style lang="scss">
.img-wrapper {
    background-color: #1c1c1c;
    font-size: 0.7rem;
    overflow: hidden;
    object-position: center;
    h2 {
        text-align: center;
    }

    p{
        text-align: center;
        margin-bottom: 2rem;
    }
}
</style>    