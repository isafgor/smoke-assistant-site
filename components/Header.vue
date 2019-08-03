<template>
  <header class="header">
      <div class="header__burger">
          <span></span>
          <span></span>
          <span></span>
      </div>
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

<script>

export default {
}
</script>

<style lang="stylus" scoped>
.header
    background #fff
    height 55px
    width 100%
    box-shadow 0 0px 16px 7px rgba(0,0,0,0.1)
    display flex
    align-items center
    justify-content space-between
    padding 0 20px
    position fixed
    @media(max-width: 1075px)
        justify-content flex-start
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
    &__burger
        display none
        margin-right 20px
        @media(max-width: 1075px)
            display block
        span 
            content ''
            display block
            width 30px
            height 3px
            margin-top 5px
            background rgba(0,0,0,0.9)
    &__menu
        display flex
        align-items center
        @media(max-width: 1075px)
            display none
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
    &__auth
        @media(max-width: 1075px)
            display none
</style>
