<script>
 
    
</script>

<template>
    <div class="wrapper-top">
        <div class="my_container">
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
        display: flex;
        justify-content: center;
    }
    h1 {
        display: flex;
        align-items: center;
        text-align: center;
        color: rgb(235, 16, 16);
    }

</style>
