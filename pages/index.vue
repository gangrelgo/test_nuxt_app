<template>
    <div class="content">
      <h1 class="title-area">Immediately regret falling into bathtub</h1>
    </div>
</template>

<script>
export default {
  layout: "default"
}
</script>

<style lang="sass" scoped>
  .title-area
    top: calc(50% - 80px)
    left: calc(50% - 375px)
    position: absolute
    font: bold 72px/80px 'Open Sans', Tahoma, serif
    font-style: normal
    text-align: center
    letter-spacing: 1.7px
    color: #FFFFFF
    display: block
    width: 750px
    height: 170px
    margin: 0
    background: linear-gradient(to right, #FFF 0%, #FFF 49.99%, #34495E 50%, #34495E 100%)
    -webkit-background-clip: text
    -webkit-text-fill-color: transparent
    @media screen and (max-width: 1200px)
      color: #FFFFFF
      -webkit-text-fill-color: #ffffff
    @media screen and (max-width: 768px)
      height: auto
      width: 100%
      top: auto
      left: auto
      background: none
      position: relative
      max-width: 100%
      -webkit-text-fill-color: #ffffff
      -webkit-background-clip: border-box
      font-size: 35px

  .content
    display: flex
    flex: 1
    width: 100%
    @media screen and (max-width: 768px)
      align-items: center
      padding: 0 20px
</style>
