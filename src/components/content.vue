<template>
  <div class="content-wrapper">
    <section class="green-section">
      <div class="green-wrapper">
        <h2>标题1</h2>
        <div class="hr"></div>
        <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
      </div>
      <div class="img">
        <i class="fa fa-diamond fa-fw fa-2x icon"></i>
        <i class="fa fa-star-o fa-fw fa-2x icon"></i>
        <i class="fa fa-heart fa-fw fa-2x icon"></i>
      </div>
    </section>
    <section id="test2" class="gray-section">
      <div class="gray-wrapper clearfix">
        <div class="section clearfix bg1">
          <div class="img">
            <img :src="pic1" alt="pic01">
          </div>
          <div class="text">
            <h2>标题2</h2>
            <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
          </div>
        </div>
        <div class="section clearfix bg2">
          <div class="text">
            <h2>标题3</h2>
            <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
          </div>
          <div class="img">
            <img :src="pic2" alt="pic01">
          </div>
        </div>
        <div class="section clearfix bg3">
          <div class="img">
            <img :src="pic3" alt="pic01">
          </div>
          <div class="text">
            <h2>标题4</h2>
            <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
          </div>
        </div>
      </div>
    </section>
    <section id="test1" class="purple-section">
      <div class="purple-wrapper clearfix">
        <div class="header">
          <h2>标题5</h2>
          <div class="hr"></div>
          <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
        </div>
        <div class="cart-group">
          <div class="card bg1">
            <h2>又一个标题</h2>
            <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
          </div>
          <div class="card bg2">
            <h2>又一个标题</h2>
            <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
          </div>
          <div class="card bg3">
            <h2>又一个标题</h2>
            <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
          </div>
          <div class="card bg4">
            <h2>又一个标题</h2>
            <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        pic1: require('../assets/pic01.jpg'),
        pic2: require('../assets/pic02.jpg'),
        pic3: require('../assets/pic03.jpg')
      }
    }
  }
</script>

<style lang="stylus">
  .green-section
    height: 700px
    background: #27ecc5
    color: white
    .green-wrapper
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
      .icon
        display: inline-block
        margin-right: 50px
        font-size: 40px
        line-height: 80px
        width: 80px
        height: 80px
        background: transparent
        font-weight: 700
        /*transform: rotate(45deg)*/
        transition: color .5s
      .icon:hover
        color: #ff4040
  .gray-section
    color: #fff
    font-size: 0
    .gray-wrapper
      .section
        .img
          display: inline-block
          width: 45%
          img
            width: 100%
        .text
          padding-top: 6%
          width: 55%
          letter-spacing: 1px
          h2
            padding-left: 5%
            font-size: 30px
            font-weight: 700
          p
            padding-left: 5%
            margin-top: 20px
            font-size: 18px
      .section > div
        float: left
      .bg1,.bg3
        background-color: #00353b
      .bg2
        background-color: #023f46
  .purple-section
    box-sizing: border-box
    background: #554075
    color: #fff
    .purple-wrapper
      width: 1080px
      margin: 0 auto
      padding-bottom: 70px
      text-align: center
      .header
        padding-top: 120px
        margin-bottom: 120px
        h2
          font-size: 30px
          font-weight: 700
          margin-bottom: 20px
      .cart-group
        width: 100%
        .card
          display: inline-block
          box-sizing: border-box
          padding-top: 100px
          width: 50%
          height: 300px
          float: left
          letter-spacing: 1px
          h2
            margin-bottom: 20px
            font-size: 28px
          p
            padding 0 30px
            font-size: 20px
        .bg1, .bg4
          background: rgba(0, 0, 0, 0.04)
        .bg2, .bg3
          background: rgba(0, 0, 0, 0.08)
</style>
