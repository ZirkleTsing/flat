<template>
  <footer>
    <div class="footer-wrapper">
      <div class="inner">
        <div class="text">
          <h2>爱我就养我</h2>
          <p>如果您觉得我的博客对您有用，请随意打赏。</p>
          <p>您的支持将鼓励我继续创作！</p>
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
          <p>如果您对我感兴趣欢迎查看<span class="resume">阿常的个人简历</span></p>
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
          p
            margin-bottom: 4px
        .button
          flex: 1 1 50%
          margin-top: 100px
          margin-left: 120px
          button
            display: block
            margin-bottom: 20px
            background: transparent
            width: 200px
            border: 3px solid #ff4040
            letter-spacing: 1px
            transition: background .5s, border-color .5s
          button:hover
            border: 3px solid #ff4040
            background: #ff4040
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
          margin-top: 40px
          p
            letter-spacing: 1px
            margin-bottom: 2px
          .resume
            color: #45D2A2
            font-weight: 700
</style>
