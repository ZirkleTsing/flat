<template>
  <div class="content-wrapper">
    <section class="green-section">
      <div class="wrapper">
        <h2>标题1</h2>
        <div class="hr"></div>
        <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
      </div>
      <div class="img">
        <span>pic1</span>
        <span>pic2</span>
        <span>pic3</span>
        <span>pic4</span>
      </div>
    </section>
    <section class="gray-section">456</section>
    <section class="purple-section">789</section>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="stylus">
  .green-section
    height: 700px
    background: #27ecc5
    color: white
    .wrapper
      padding-top: 200px
      width: 1080px
      margin: 0 auto
      text-align: center
      letter-spacing: 1px
      h2
        padding-bottom: 20px
        font-weight: 700
        font-size: 30px
      .hr
        height: 2px
        margin: 0 auto
        width: 55%
        background: #fff
      p
        margin-top: 20px
        font-size: 18px
    .img
      width: 1080px
      margin: 0 auto
      padding-top: 160px
      text-align: center
      span
        margin-right: 20px
        font-size: 20px
</style>
