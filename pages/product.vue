<template>
  <div class="content">
    <div class="content-area">
      <div class="main-text-area">
        <h1 class="cases">Study case</h1>
        <p class="case-text">
          Run in circles show belly, lick paws
          then retire to the warmest spot on the couch
          to claw at the fabric.
        </p>
      </div>
      <hooper
        :infiniteScroll="true"
        :shortDrag="true"
        class="main-image-area" >
        <slide
          class="img-container"
          v-for="image in pictures"
          :key="image.id">
          <img class="case-pict" draggable="false" :src="image.picture">
        </slide>

      </hooper>
    </div>
  </div>
</template>

<script>
  import { Hooper, Slide } from 'hooper';
  import 'hooper/dist/hooper.css';
  export default {
    name: 'App',
    components: {
      Hooper,
      Slide,
    },
    data() {
      return {
        pictures: [
          {id: 0, picture: "/img/caseimage.png"},
          {id: 1, picture: "/img/caseimage-2.jpg"},
          {id: 2, picture: "/img/caseimage-3.jpg"}
        ]
      }
    }
  }

</script>

<style lang="sass" scoped>
  .main-text-area
    margin: 168px auto auto 70px
    position: relative
    z-index: 2
    width: 370px
    @media screen and (max-width: 1600px)
        margin: 168px auto auto -98px
    @media screen and (max-width: 1200px)
      text-align: center
      margin: calc(20% - 160px ) auto 0 auto
      width: 100%

  .content
    display: flex
    flex: 1
    width: 100%

  .cases
    font-family: Open Sans, sans-serif
    font-style: normal
    font-weight: bold
    line-height: 87px
    font-size: 64px
    letter-spacing: 3px
    color: #FFFFFF
    @media screen and (max-width: 1200px)
      font-size: 50px

  .content-area
    padding: 0 230px 0 140px
    position: relative
    height: 100%
    width: 100%
    @media screen and (max-width: 1200px)
      padding: 0

  .case-text
    font-family: Open Sans, sans-serif
    font-style: normal
    font-weight: 300
    line-height: 23px
    font-size: 16px
    letter-spacing: 0.72px
    color: #ECF0F1
    width: 201px
    height: auto
    user-select: none
    @media screen and (max-width: 1200px)
      width: 100%


  .case-pict
    width: 100%
    height: auto
    margin: 0
    padding: 0


  .main-image-area
    position: absolute
    top: 98px
    right: 255px
    height: 515px
    width: 900px
    user-select: none
    outline: none
    @media screen and (max-width: 1600px)
      left: 23%
    @media screen and (max-width: 1200px)
      position: relative
      margin: auto auto 0
      left: 0
      top: 0
      width: auto
      max-width: 750px




</style>
