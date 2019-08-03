<template>
  <header class="header">
       <div class="header__logo">
           <router-link to="/">#где<span>Покурить</span></router-link>
       </div>
       <div class="header__menu">
           <div class="header__menu-link">
               <router-link to="/">Главная</router-link>
           </div>
           <div class="header__menu-link">
               <router-link to="/all-hokaah">Все заведения</router-link>
           </div>
           <div class="header__menu-link">
               <router-link to="/about">О сервисе</router-link>
           </div>
       </div>
       <div class="header__auth">
           <el-button>Войти</el-button>
           <el-button class="header__signup">Зарегистрироваться</el-button>
       </div>
  </header>
</template>

<style lang="stylus" scoped>
.header
    background #fff
    height 55px
    box-shadow 0 0px 16px 7px rgba(0,0,0,0.1)
    display flex
    align-items center
    justify-content space-between
    padding 0 20px
    position relative
    &__signup
        background #41b883
        border-color #41b883
        color #fff
    &__logo
        font-size 25px
        font-weight 500
        cursor pointer
        a
            color #000
            text-decoration none
        span
            color #41b883
    &__menu
        display flex
        align-items center
    &__menu-link
        margin-left 20px
        a
            color rgba(0, 0, 0, .7)
            text-decoration none
            font-size 17px
            font-weight 500
            transition .5s
            &:hover
                color rgba(0, 0, 0, 1)
</style>
