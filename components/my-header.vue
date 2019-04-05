<template>
  <div class="header">
    <div class="half-side"></div>
    <div class="half-side p-left-social">
      <h2 class="page-title" :class="{'page-title-dark':isWhiteTheme}" > {{ changeTitle }}</h2>
    </div>
  </div>
</template>

<script>
  export default {      //@-ссылка на корень проекта
    name: "myHeader",
    props: {

    },
    data() {        //локальные переменные
      return {
        titleText: "Let's get started"
      }
    },
    mounted() {

    },
    computed: {
      isWhiteTheme(){
        return !!(this.$route.name === "about" || this.$route.name === "contacts")
      },
      changeTitle(){
        if (this.$route.name === "index") return this.titleText = "Let's get started"
        else if (this.$route.name === "about") return this.titleText = "Who we are"
        else if (this.$route.name === "product") return this.titleText = "What we do"
        else return this.titleText = "Get in touch"
      }
    },
    methods: {
    }
  }
</script>

<style lang="sass" scoped>
  .header
    height: 50px
    width: 100%
    display: flex
    flex-direction: row
    padding-top: 33px
    .half-side
      position: relative
      width: 50%
      display: flex
      justify-content: center
      z-index: 1
      @media screen and (max-width: 1200px)
        display: none
    .p-left-social
      position: relative
      padding-left: 140px
      z-index: 1
      @media screen and (max-width: 1200px)
        display: block
        width: 100%
        padding: 0

  .page-title
    display: block
    font: 800 12px/15px 'Merriweather Sans', Tahoma, serif
    letter-spacing: 0.7px
    text-transform: uppercase
    color: #34495E
    text-decoration: none
    @media screen and (max-width: 1200px)
      color: #ffffff
      text-align: center
      .container-column-white &
        color: #34495E
  .page-title-dark
    color: #ECF0F1



</style>

