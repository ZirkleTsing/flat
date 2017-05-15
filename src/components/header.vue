<template>
  <header>
    <div class="header-wrapper">
      <nav>
        <h1 id="header-info">
          <a id="header-info-address" href="#">常小窝</a>
          <i class="fa fa-home fa-fw"></i>
        </h1>
        <ul id="header-list">
          <li @click="chooseList(index)" class="list" v-for="(item, index) in navList">
            <a :class="{'active': currentIndex === item.index}" :href="item.address">{{ item.text }}
            </a>
            <i :class="{'fa fa-reorder': index === 1}" class="home"></i>
          </li>
        </ul>
      </nav>
      <div class="banner">
        <div class="inner">
          <h2 id="brand">常小窝</h2>
          <p id="desc">来自2060的阿常</p>
          <button @click="scrolldown" id="banner-button">了解我</button>
<!--          <div class="more">更多</div>-->
          <a class="arrow" href="#overview"><i class="fa fa-arrow-down fa-3x arrow "></i></a>
        </div>
      </div>
    </div>
    <audio src="http://link.hhtjim.com/163/28586064.mp3" id="audio1" hidden="true" autoplay="true" loop="true">
    </audio>
  </header>
</template>

<script>
  import $ from 'jquery'

  export default {
    data () {
      return {
        navList: [
          {
            text: '首页',
            address: '#',
            index: 0
          },
          {
            text: '导航',
            address: '#',
            index: 1
          }
        ],
        currentIndex: 0
      }
    },
    methods: {
      chooseList (index) {
        this.currentIndex = index
      },
      scrolldown () {
        $('html,body').animate({
          scrollTop: $($('a.arrow').attr('href')).offset().top + 'px'
        }, {
          duration: 800,
          easing: 'swing'
        })
        return false
      }
    },
    mounted () {
      $(document).ready(function () {
        $('a.arrow').click(function () {
          $('html,body').animate({
            scrollTop: $($(this).attr('href')).offset().top + 'px'
          }, {
            duration: 800,
            easing: 'swing'
          })
          return false
        })
      })
    }
  }
</script>

<style lang="stylus" scoped>
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
      animation: headerInfo 3s
    i
      transition: opacity .3s linear
      opacity: 0
      font-size: 30px
  #header-info:hover
    i
      opacity: 1
      font-size: 30px
  #header-list
    display: inline-block
    float: right
    padding: 10px 15px
  .list
    positon: relative
    display: inline-block
    margin-right: 12px
    font-size: 25px
  .list a
    display:inline-block
    position: relative
    margin-right: 2px
    padding: 0 5px 5px 5px
    letter-spacing: 1px
    color: #fff
    animation: headerInfo 3s
  .active:after
    display: block
    position: absolute
    bottom: 0
    left: 0%
    width: 100%
    content: ''
    border-bottom: 3px solid #fff
    animation: navList .3s linear
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
      p
        font-weight: 700
        letter-spacing: 1px
      #brand
        position: relative
        display: block
        margin-bottom: 20px
        padding: 10px 0px
        font-size: 35px
 //       border-top: 3px solid #fff
 //       border-bottom: 3px solid #fff
      #brand:after
        display: block
        position: absolute
        content: ''
        bottom: 0
        left: 15%
        right: 15%
        width: 70%
        border-bottom: 3px solid #fff
        animation: borderShow 1s linear
      #brand:before
        display: block
        position: absolute
        content: ''
        top: 0
        left: 15%
        right: 15%
        width: 70%
        border-top: 3px solid #fff
        animation: borderShow 1s linear
      #banner-button
        margin-top: 20px
        width: 210px
        background: transparent
        border: 3px solid #ff4040
        letter-spacing: 3px
        color: #fff
        transition: background .5s, border-color .5s
      #banner-button:hover
        background: #ff4040
        border: 3px solid #ff4040
      .more
        font-size: 30px
        font-weight: 700
        margin-top: 100px
      .arrow
        display: block
        margin-top: 140px
        color: #fff
        animation: arrow 1s infinite alternate
</style>
