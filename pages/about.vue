<template>
    <div class="content">
      <div class="small-circle">

      </div>
      <div class="half-content">
        <div class="about-left-content">
          <i class="fas fa-quote-left">
          </i>
          <span class = "my-left-donut">
            My left donut is missing, as is my right destroy the blinds. Cat snacks cough hairball on conveniently placed pants cough furball for scratch at fleas scratch strangers and dream about hunting birds.
          </span>
        </div>
      </div>
      <div class="half-content">
        <div class = text-area>
          <p class = 'paragraph'>
            Run outside as soon as door open. Eat all the power cords refuse to drink water except out of someone's glass purr so eat all the power cords but purr, and sit on human meow. Dream about hunting birds. Kitty kitty kitty poochy, yet intrigued by the shower.
          </p>
          <p class = 'paragraph'>
            Hiss and stare at nothing then run suddenly away. Stare out the window destroy couch, and meow meow loudly just to annoy owners for spit up on light gray carpet instead of adjacent linoleum but need to chase tail. Stare out the window nap all day claw drapes ask for petting and make a weird face.
          </p>
          <p class = 'paragraph'>
            Knock dish off table rub face on owner need to chase tail, yet freak human out make funny noise mow mow mow mow mow mow success now attack human, attack feet. Present belly, scratch hand when stroked pounce on unsuspecting person yet chase mice. Hide head under blanket so no one can see. Slap owner's face until human fills food dish.
          </p>
        </div>
      </div>
    </div>
</template>

<script>
  export default {
    layout: "default"
  }
</script>

<style lang="sass" scoped>
  .fa-quote-left
    position: relative
    color: #34495E
    display: block
    height: 50px
    font-size: 48px
    margin: 0
    z-index: 3

  .content
    display: flex
    flex: 1
    width: 100%
    @media screen and (max-width: 1200px)
      align-items: center
      padding: 0 20px
      display: flex
      flex-direction: column


  .content-area
    padding: 0 230px 0 140px
    position: relative
    height: 100%
    width: 100%

  .half-content
    width: 50%
    height: 100%
    align-items: center
    @media screen and (max-width: 1200px)
      height: auto
      width: 100%
      margin: 0
      align-items: center

  .about-left-content
    display: flex
    flex-direction: column
    width: 60%
    margin: 220px auto 0 230px
    @media screen and (max-width: 1200px)
      margin: 50px auto 0;
      width: 75%


  .my-left-donut
    position: relative
    text-shadow: 0 3px 3px #ccc
    font: 600 18px/25px 'Merriweather Sans', Tahoma, serif
    font-style: normal
    text-align: left
    letter-spacing: 1.3px
    color: #34495E
    height: auto
    padding: 0
    z-index: 3
    margin-top: 35px
    @media screen and (max-width: 1200px)
      width: 100%


  .text-area
    position: relative
    width: 400px
    margin-left: 25%
    margin-top: 125px
    @media screen and (max-width: 1200px)
      width: 75%
      margin: 100px auto 0


  .paragraph
    font-family: Merriweather Sans, sans-serif
    font-style: normal
    font-weight: 400
    line-height: 21px
    font-size: 15px
    letter-spacing: 1.2px
    color: #ECF0F1
    @media screen and (max-width: 1200px)
      color: #34495E



  .small-circle
    position: absolute
    width: 90px
    height: 90px
    border-radius: 50%
    box-shadow: 0 0 0 3px rgba(52, 73, 94, .03), 0 0 0 48px #ECF0F1, 0 0 0 52px rgba(52, 73, 94, .03), 0 0 0 92px #ECF0F1, 0 0 0 97px rgba(52, 73, 94, .03), 0 0 0 142px #ECF0F1, 0 0 0 148px rgba(52, 73, 94, .03)
    top: calc(50% - 45px)
    left: 25%
    background: transparent
    @media screen and (max-width: 1200px)
      left: calc(50% - 45px)
      top: calc(50% - 45px)

</style>
