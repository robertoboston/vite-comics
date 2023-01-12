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
        <div class="container">
            <a href="/" class="Logo">
             <img src="../assets/img/dc-logo.png" alt="">
            </a>
            <nav>
              <ul>
                    <li v-for="(item,index) in menu " :key="index" :class="item.active == true ? 'active' : '' ">
                    <a :href="item.url">{{item.label}}</a>
                    </li>
              </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header{
   width: 100%;
   height: 100px;
   @include flex-centered;

   .container{
    width: 1200px;
    @include flex-between;
   }

   .logo{
    margin: 1rem 0;
   }

   nav{
    width: 60%;
    height: 100%;
   }

    ul{
        list-style: none;
        height: 100%;
        display: flex;
        @include flex-between;
        text-transform: uppercase;
        


        li{
            padding: 0 20px;
            height: 100%;

            &.active,
            &:hover{
                border-bottom: 2px  solid blue;
            }

            a{
                text-decoration: none;
                align-items: center;
                @include flex-centered;
                height: 100%;
            }
            
        }
    }

}



    
</style>