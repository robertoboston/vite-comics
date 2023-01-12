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
    <footer>
        <div class="background-image-footer">
            <div class="container">
                <nav>
                    <h2>Dc comics</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Moovies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </nav>
             


            </div>
        </div>
    </footer>
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

.background-image-footer{
    background-image: url(../assets/img/footer-bg.jpg);
    width: 100%;
    background-size: cover;
    background-repeat: no-repeat;
    @include flex-centered;

    .container{
        height: 500px;
        width: 100%;
    }

 
    
}
    
</style>