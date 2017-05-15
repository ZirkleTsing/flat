<template>
  <div class="content-wrapper">
    <section id="overview" class="green-section">
      <div class="green-wrapper">
        <h2>关于我  <i class="fa fa-heart fa-fw icon"></i></h2>
        <div class="hr"></div>
        <div class="text">
          <p>常用昵称阿常先森活跃于各大网站，来自<span class="school">北京工业大学</span>，在读大三本科生</p>
          <p>90后处女座男青年，爱折腾，喜欢游弋在代码中那种简简单单的感觉</p>
          <p>相信代码是一种艺术，编程是一种生活态度。</p>
          <p>前端渣渣一枚，目前为止仍在找寻属于自己的Coding之路</p>
          <p>Fighting!!!</p>
        </div>
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
    height: 1000px
    background: rgba(0, 0, 0, 0.4)
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
        .icon
          color: #fff
          transition: color .5s
        .icon:hover
          color: #ff4040
      .hr
        height: 2px
        margin: 0 auto
        width: 55%
        background: #fff
      .text
        padding: 10px 230px
      p
        margin-top: 20px
        font-size: 18px
        .school
          color: #45D2A2
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
