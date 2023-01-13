<script>
import comicsData from '../assets/data/datacomics.js';
import AppComics from './AppComics.vue'

export default {
    components :{
        AppComics

    },
    data(){
        return {
            comics: comicsData 
        }
    }
    
}
</script>

<template lang="">
    <div class="dark-bg">
            <div class="title-section">
                <h2 class="title">Comics Series</h2>
            </div>
        <div class="section-fumetti">
            <div class="comics-container">
                <AppComics v-for="(item, index) in comics" :key="index" :comic="item"></AppComics>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

.dark-bg{
    background-color: rgb(33, 33, 33);
}


.title-section{
    position: relative;

}

.title{
    text-transform: uppercase;
    color: white;
    position: absolute;
    top: -25px;
    background-color: $primary;
    width: 250px;
    padding: 15px;
    margin-left: 100px;
    text-align: center;
}

.section-fumetti{
    width: 70%;
    margin: 0 auto;
    display: flex
}

.comics-container{
    width: 100%;
    @include flex-v-center;
    justify-content: space-between;
    flex-wrap: wrap;
    padding-top: 5rem
}



    
</style>