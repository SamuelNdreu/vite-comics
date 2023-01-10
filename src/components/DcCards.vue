<script>
export default {
    props: [
        'thumbnail',
        'price',
        'series',
        'type'
    ]
}
</script>

<template>
    <div>
        <div class="img-wrapper">
            <img :src="thumbnail">
        </div>
        <p>{{ series }}</p>
    </div>
</template>

<style lang="scss">
    .img-wrapper{
    margin-top: 1rem;
    
    overflow: hidden
    }
</style>    