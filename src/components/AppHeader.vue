<script>
export default {
    data(){
        return{
            menu : [
                {
                    label : 'characters',
                    url : '#',
                    active : false
                },
                {
                    label : 'comics',
                    url : '#',
                    active : true,
                },
                {
                    label : 'movies',
                    url : '#',
                    active : false
                },
                {
                    label : 'tv',
                    url : '#',
                    active : false
                },
                {
                    label : 'games',
                    url : '#',
                    active : false
                },
                {
                    label : 'collectibles',
                    url : '#',
                    active : false
                },
                {
                    label : 'videos',
                    url : '#',
                    active : false
                },
                {
                    label : 'fans',
                    url : '#',
                    active : false
                },
                {
                    label : 'news',
                    url : '#',
                    active : false
                },
                 {
                    label : 'shop',
                    url : '#',
                    active : false
                }
            ]
        }
    }
    
}
</script>

<template lang="">
    <header>
        <a href="/" class="Logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </a>
        <nav>
            <ul>
                <li v-for="(item,index) in menu " :key="index">
                    <a :href="item.url">{{item.label}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;

header{
    display: flex;
    justify-content: space-around;
    align-items: center;

    ul{
        list-style: none;
        display: flex;
        


        li{
            padding: 0 20px;

            a{
                text-decoration: none;
                color: $primary;
            }
            
        }
    }

}



    
</style>