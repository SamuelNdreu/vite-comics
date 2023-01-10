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
        </div>
        <p>{{ series }}</p>
    </div>
</template>

<style lang="scss">
.img-wrapper {
    background-color: #1c1c1c;

    overflow: hidden;
}
</style>    