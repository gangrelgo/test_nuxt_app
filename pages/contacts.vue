<template>
  <div class="content">
    <div class="half-content">
      <div class="form">
        <form class="page-form" onsubmit="validate(event)">
          <input id="firstField" class="text-form" required placeholder="Name">
          <input id="secondField" type="email" class="text-form" required placeholder="E-mail">
          <input id="thirdField" type="tel" class="text-form" required placeholder="Number">
          <textarea id="fourthField" class="text-message" required placeholder="Message"></textarea>
          <button type="submit" class="submit">
            <span class="sub-text"> submit </span>
            <img class="sub-pict" src="@/assets/shape.png">
          </button>
        </form>
      </div>
    </div>
    <div class="half-content">
      <iframe class="map" src="https://yandex.ru/map-widget/v1/?um=constructor%3A6e77977a1b9ccf03d0d59a733e0b4df13a56bd5808f353399a830b310545511a&amp;source=constructor" width="100%" height="720" frameborder="0"></iframe>
    </div>
  </div>
</template>

<script>
  export default {
    layout: "default"
    }

</script>

<style lang="sass" scoped>
  .content
    display: flex
    flex: 1
    width: 100%
    @media screen and (max-width: 1600px)
      align-items: center
      padding: 0 20px


  .half-content
    width: 50%
    height: 100%
    align-items: center
    @media screen and (max-width: 1200px)
      height: auto
      width: 100%
      margin: 0
      align-items: center
  .form
    display: flex
    flex-direction: column
    margin-left: 238px
    margin-top: 85px
    position: relative


  .text-form
    font-family: Open Sans, sans-serif
    font-style: normal
    font-weight: bold
    line-height: 19px
    font-size: 14px
    color: #ECF0F1
    background: #34495E
    border: 1px solid #34495E
    border-radius: 27px
    width: 325px
    height: 55px
    padding-left: 25px

  .map
    margin-top: -50px
    margin-bottom: 0
    height: 820px
    z-index: 0
  .text-message
    font-family: Open Sans, sans-serif
    font-style: normal
    font-weight: bold
    line-height: 19px
    font-size: 14px
    color: #ECF0F1
    background: #34495E
    border: 1px solid #34495E
    border-radius: 27px
    width: 325px
    height: 168px
    padding-left: 25px


  .page-form
    width: 352px


  .page-form input, textarea
    margin-bottom: 35px

  .submit
    background: #ECF0F1
    width: 350px
    height: 55px
    border: 2px solid #34495E
    border-radius: 27px
    padding-left: 25px
    display: flex
    flex-direction: row


  .sub-pict
    padding-left: 4px


  .sub-text
    font: 700 19px/14px 'Open Sans', sans-serif
    color: #34495E
    padding-left: 120px
    font-size: 14px


  .text-form::-webkit-input-placeholder
    color: #ECF0F1

  .text-message::-webkit-input-placeholder
    color: #ECF0F1

</style>
