<template>
  <section id="main-area">
    <div class="container" :class="{'container-column-white':isWhiteTheme}">
      <my-header/>
      <nuxt/>
      <my-footer/>
    </div>
  </section>
</template>


<script>
import MyHeader from "@/components/my-header"
import MyFooter from "@/components/my-footer"
export default {
  components: {
    MyHeader,
    MyFooter

  },
  name: "default",
  props: {

  },
  data() {
    return {

    }
  },
  mounted() {

  },
  computed: {
    isWhiteTheme(){
      return !!(this.$route.name === "about" || this.$route.name === "contacts")
    }
  },
  methods: {

  }
}
</script>

<style lang="sass">
  html, body
    padding: 0
    margin: 0
    box-sizing: border-box
    height: 100%
    min-height: 100%


  div
    box-sizing: border-box

  #__nuxt, #__layout
    padding: 0
    margin: 0
    box-sizing: border-box
    height: 100%
    min-height: 100%

  #main-area
    height: 100%
    min-height: 100%
    background: #ffffff
    display: flex
    justify-content: center
    align-items: center


  .container
    overflow: hidden
    height: 820px
    width: 1600px
    display: flex
    position: relative
    flex-direction: column
    background: linear-gradient(to right, #34495E 0%, #34495E 49.99%, #ECF0F1 50%, #ECF0F1 100%)
    @media screen and (max-width: 1200px)
      background: #34495E
      width: 100%
      height: 100%
      .container-column-white &
        background: #ECF0F1


  .container-column-white
    background: linear-gradient(to right, #ECF0F1 0%, #ECF0F1 49.99%, #34495E 50%, #34495E 100%)
    @media screen and (max-width: 1200px)
     background: #ECF0F1

</style>
