<script>
export default {
    
}
</script>

<template lang="">
    <div class="blue-row">
        <div class="container">
            <div class="mini-container">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="/">
            <h1>Digital Comics</h1>
        </div>
        <div class="mini-container">
            <img src="../assets/img/buy-comics-merchandise.png" alt="/">
            <h1>Digital Comics</h1>
        </div>
        <div class="mini-container">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="/">
            <h1>Digital Comics</h1>
        </div>
        <div class="mini-container">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="/">
            <h1>Digital Comics</h1>
        </div>
        <div class="mini-container">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="/">
            <h1>Digital Comics</h1>
        </div>
        </div>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

.blue-row{
    @include blue-sets;
    background-color: $primary;
    display: flex;
    justify-content:center;
    align-items: center;

    .container{
        display: flex;
    }

    .mini-container{
        width: calc(100% / 5);
        display: flex;
        align-items: center;
        margin: 40px;
        color: white;
    }

    img{
        height: 80px;
    }

    h1{
        font-size: 15px;
        padding: 15px;
    }

}
    
</style>