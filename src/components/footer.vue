<template>
  <footer>
    <div class="footer-wrapper">
      <div class="inner">
        <div class="text">
          <h2>爱我就养我</h2>
          <p>Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
        </div>
        <div class="button">
          <button>给钱</button>
          <button>给吃的</button>
        </div>
      </div>
      <div class="bottom">
        <ul class="share-group">
          <li><i class="fa fa-github fa-2x fa-fw"></i></li>
          <li><i class="fa fa-wechat fa-2x fa-fw"></i></li>
          <li><i class="fa fa-weibo fa-2x fa-fw"></i></li>
          <li><i class="fa fa-facebook fa-2x fa-fw"></i></li>
        </ul>
        <div class="copy">
          <p>&copy 来自未来的阿常 - 2060.5.12</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
  export default {}
</script>

<style lang="stylus">
  footer
    background: rgba(0, 0, 0, 0.4)
    color: #fff
    .footer-wrapper
      .inner
        display: flex
        margin: 0 auto
        width: 1080px
        min-height: 300px
        letter-spacing: 1px
        .text
          flex: 1 1 50%
          margin-top: 130px
          text-align: center
          h2
            margin-bottom: 20px
            font-size: 30px
            font-weight: 700
        .button
          flex: 1 1 50%
          margin-top: 100px
          margin-left: 120px
          button
            display: block
            margin-bottom: 20px
            width: 200px
            border: 2px solid #fff
            letter-spacing: 1px
      .bottom
        box-sizing: border-box
        min-height: 200px
        background: rgba(3, 3, 3, 0.4)
        text-align: center
        .share-group
          display: block
          margin: 0 auto
          padding-top: 70px
          width: 1080px
          li
            display: inline-block
            padding: 0 15px
            i
              color: #fff
              transition: color .3s
            i:hover
              color: #333
        .copy
          margin-top: 60px
          p
            letter-spacing: 1px
</style>
