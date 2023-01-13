<script>
export default {
    props: {
        comic : Object
    }
    
}
</script>

<template lang="">
    <div>
        <div class="comics-card">
            <div class="thumb-container">
                <img :src="comic.thumb" class="thumb" :alt="comic.series">
            </div>
            <div class="title-container">
                 <h4>{{comic.series}}</h4>
                 <h4>{{comic.price}}</h4>
                 <h4>{{comic.type}}</h4>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>



    
</style>