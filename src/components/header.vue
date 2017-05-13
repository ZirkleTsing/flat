<template>
  <header>
    <div class="header-wrapper">
      <nav>
        <h1 id="header-info">
          <a id="header-info-address" href="#">常小窝</a>
        </h1>
        <ul id="header-list">
          <li class="list" v-for="item in navList">
            <a :href="item.address">{{ item.text }}</a>
          </li>
        </ul>
      </nav>
      <div class="banner">
        <div class="inner">
          <h2 id="brand">常小窝</h2>
          <p id="desc">Lorem ipsum dolor sit amet, consecterur adipisicing elit.</p>
          <button id="banner-button">了解我</button>
          <div class="more">更多</div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
    data () {
      return {
        navList: [
          {
            text: '首页',
            address: '#'
          },
          {
            text: '导航',
            address: '#'
          }
        ]
      }
    }
  }
</script>

<style lang="stylus">
  .header-wrapper
    position: relative
    color: #fff
  nav
    height: 50px
    background: rgba(0, 0, 0, 0.4)
  #header-info
    display: inline-block
    box-sizing:border-box
    padding: 10px 15px
    line-height: 30px
    font-size: 25px
    letter-spacing: 1px
    #header-info-address
      color: #fff
  #header-list
    display: inline-block
    float: right
    padding: 15px 15px
  .list
    display: inline-block
    font-size: 20px
  .list a
    margin-right: 10px
    letter-spacing: 1px
    color: #fff
  .banner
    height: 1000px
    background: rgba(0, 0, 0, 0.4)
    .inner
      margin: 0 auto
      box-sizing: border-box
      padding-top: 300px
      width: 300px
      text-align: center
      letter-spacing: 1px
      #brand
        display: block
        margin-bottom: 20px
        padding: 10px 0px
        font-size: 35px
        border-top: 3px solid #fff
        border-bottom: 3px solid #fff
      #banner-button
        margin-top: 20px
        width: 200px
      .more
        font-size: 18px
        margin-top: 260px
</style>
