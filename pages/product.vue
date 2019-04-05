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
      <div class="main-image-area">
        <img class="case-pict" src="@/assets/caseimage.png">
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {

      }
  }

</script>

<style lang="sass" scoped>
  .main-text-area
    margin: 168px auto auto 70px
    position: relative
    z-index: 2
    @media screen and (max-width: 1600px)
        margin: 168px auto auto -98px
    @media screen and (max-width: 768px)
      text-align: center
      margin: calc(20% - 127px ) auto 0 auto
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

  .content-area
    padding: 0 230px 0 140px
    position: relative
    height: 100%
    width: 100%
    @media screen and (max-width: 768px)
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
    height: 115px
    @media screen and (max-width: 768px)
      width: 100%

  .case-pict
    width: 100%
    height: 100%
    margin: 0
    padding: 0


  .main-image-area
    position: absolute
    top: 98px
    right: 255px
    height: 515px
    width: 900px
    @media screen and (max-width: 1600px)
      left: 23%
    @media screen and (max-width: 1200px)
      top: 156px
      right: 255px
      height: 343px
      width: 580px
    @media screen and (max-width: 768px)
      position: relative
      left: 0
      top: 0
      width: 100%
      height: auto
      margin: calc(35% - 200px) auto 0
</style>
