<template>
  <div class="footer">
    <div class="half-side">
      <nav class="menu-column">
        <ul class="menu-list">
          <li class="menu-item">
            <nuxt-link
              to="/"
              class="menu-link">Main</nuxt-link>
          </li>
          <li class="menu-item">
            <nuxt-link
              to="/about"
              class="menu-link">About</nuxt-link>
          </li>
          <li class="menu-item">
            <nuxt-link
              to="/product"
              class="menu-link">Products</nuxt-link>
          </li>
          <li class="menu-item">
            <nuxt-link
              to="/contacts"
              class="menu-link">Contacts</nuxt-link>
          </li>
        </ul>
      </nav>
    </div>
    <div class="half-side p-left-social">
      <ul class="social-list">
        <li class="social-item">
          <a
            class="social-link"
            href="#"
            target="_blank">
            <i class="fab fa-twitter"></i>
          </a>
        </li>
        <li class="social-item">
          <a
            class="social-link"
            href="#"
            target="_blank">
            <i class="fab fa-linkedin-in"></i>
          </a>
        </li>
        <li class="social-item">
          <a
            class="social-link"
            href="#"
            target="_blank">
            <i class="fab fa-facebook"></i>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {      //@-ссылка на корень проекта
    name: "Myfooter",
    props: {

    },
    data() {        //локальные переменные
      return {

      }
    },
    computed: {
      isWhiteTheme(){
        return !!(this.$route.name === "about" || this.$route.name === "contact")
      },
    mounted() {

    },

    },
    methods: {

    }
  }
</script>

<style lang="sass" scoped>
  .footer
    display: flex
    flex-direction: row
    height: 100px
    width: 100%
    position: relative
    z-index: 1
    flex: 0 1 auto
  .half-side
    position: relative
    width: 50%
    display: flex
    justify-content: center
    z-index: 1
    @media screen and (max-width: 768px)
      width: 100%

  .menu-column
    margin: 0
    padding: 0
    &.menu
      margin: 720px 0 0
      text-align: center
    .menu-list
      padding: 0
      margin: 0



  .menu-item
    display: inline-block
    margin-left: 40px
    &:first-child
      margin-left: 0
    .menu-link
      font: bold 12px/15px 'Merriweather Sans', Tahoma, serif
      letter-spacing: 1.2px
      text-transform: uppercase
      color: #ECF0F1
      text-decoration: none
      position: relative
      .container-column-white &
        color: #34495E
      &:hover
        &:before
          background: #ECF0F1
          display: block
      &:before
        content: ''
        position: absolute
        display: none
        width: 44px
        height: 3px
        top: calc(50% - 2px)
        left: calc(50% - 22px)
        transform: rotate(-45deg)
        background: #FFFFFF
        text-decoration: underline
        .container-column-white &
          background: #34495E


  .nuxt-link-exact-active
    &.menu-link
      &:before
        display: block

  .p-left-social
    position: relative
    padding-left: 140px
    z-index: 1
    @media screen and (max-width: 768px)
      padding: 0
      margin-top: 10px

  .social-list
    padding: 0
    margin: 0
    &.social-list-white
      padding-left: 220px
    .social-item
      display: inline-block
      margin-left: 20px
      &:first-child
        margin-left: 0
      .social-link
        display: block
        width: 23px
        height: 23px
        text-align: center
        border-radius: 50%
        border: 2px solid #34495E
        text-decoration: none
        @media screen and (max-width: 1200px)
          border-color: #ffffff
        .container-column-white &
          border-color: #ffffff
          @media screen and (max-width: 1200px)
            border-color: #34495E
        .fab
          color: #34495E
          font-size: 14px
          line-height: 23px
          @media screen and (max-width: 1200px)
            color: #ffffff
          .container-column-white &
            color: #ffffff
            @media screen and (max-width: 1200px)
              color: #34495E
        &:hover
          .fab
            color: darkred

  .footer
    @media screen and (max-width: 768px)
      flex-direction: column
</style>
