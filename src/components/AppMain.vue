<script>
export default {
    
}
</script>

<template lang="">
    <div class="background-black">
        <h1>'Content goes here'</h1>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/mixins' as *;

.background-black{
    height: 150px;
    width: 100%;
    background-color: black;
    color: white;
    @include flex-centered;
    align-items: center;
}

    
</style>