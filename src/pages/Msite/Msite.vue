<template>
    <div class="msite">
        <header class="header">
          <div class="dingwei">
            <span><i class="iconfont iconicon-dingwei"></i></span>
            <a class="weizhi">雄楚大道666号...</a>
          </div>
          <i class="iconfont iconsearch on"></i>
          <input class="search" type="text" placeholder="搜索饿了么商家、商品名称"/>
        </header>
        <nav class="nav-w">
          <ul class="nav">
            <li class="listarr" v-for="(item,key) in navdata">
              <a class="nav-a" href="#" >
                <img class="image" v-bind:src="item.imgarr"/>
                <p class="nav-name">{{item.name}}</p>
              </a>
            </li>
          </ul>
        </nav>
        <section class="banner-w">
          <a href="#" class="banner-a">
            <div class="banner-l">
              <h1 class="one">品质套餐</h1>
              <p class="two">搭配齐全吃得好</p>
              <p class="three">立即抢购 ></p>
            </div>
            <img class="banner-r" src="./img/xiaochaorou.jpg"/>
          </a>
        </section>
        <footer class="footer-w">
            <p class="footer-p">— 推荐商家 —</p>
            <ul class="footer-u">
              <li>综合排序</li>
              <li>距离最近</li>
              <li>销量最高</li>
              <li>筛选</li>
            </ul>
            <img src="./img/waimaixiaoge.jpg"/>
        </footer>
    </div>
</template>

<script>
export default {
  data () {
    return {
      navdata:[
        {
          imgarr:require("./img/1.png"),
          name:'美食'
        },
        {
          imgarr:require("./img/2.png"),
          name:'晚餐'
        },
        {
          imgarr:require("./img/3.png"),
          name:'跑腿代购'
        },
        {
          imgarr:require("./img/4.png"),
          name:'汉堡披萨'
        },
        {
          imgarr:require("./img/5.png"),
          name:'甜品饮品'
        },
        {
          imgarr:require("./img/6.png"),
          name:'地方小吃'
        },
        {
          imgarr:require("./img/7.png"),
          name:'米粉面馆'
        },
        {
          imgarr:require("./img/8.png"),
          name:'包子粥店'
        },
        {
          imgarr:require("./img/9.png"),
          name:'炸鸡炸串'
        },
        {
          imgarr:require("./img/10.png"),
          name:'品质套餐'
        },
      ]
    }
  }

}
</script>

<style lang="stylus" rel="stylesheet/stylus">
.msite
  width 100%
  height 100%+20px
  .header
    position relative
    height 75px
    background-color deepskyblue
    font-size 16px
    color white
    .dingwei
      line-height 15px
      padding 10px
    .on
      position absolute
      z-index 2
      color #779dbd
      left 80px
      top 45px
    .search
      width 90%
      height 25px
      margin 5px 4.5%
      border none
      text-align center
  .nav-w
    width 100%
    height 180px
    .nav
      display flex
      justify-content center
      align-items center
      flex-wrap wrap
      .listarr
        flex 1
        padding 10px
        .nav-a
          text-decoration none
          .image
            width 50px
            height 50px
          .nav-name
            font-size 12px
            text-align center
            color #779dbd
  .banner-w
    height 120px
    width 95%
    margin 0 auto
    background-color #d9d9d9
    .banner-a
      text-decoration none
      .banner-l
        float left
        width 150px
        margin 15px 0 0 15px
        .one
          font-size 20px
          color black
        .two
          font-size 15px
          margin 10px 0
          color #777777
        .three
          font-size 12px
          color #BC7A00
      .banner-r
        float right
        width 150px
        margin 15px 15px 0 0


  .footer-w
    width 100%
    .footer-p
      text-align center
      margin 20px 0
    .footer-u
      display flex
      li
        flex 1
        text-align center
        flex-direction column
        align-items center
        font-size 14px
    img
      width 50%
      margin-top 35px
      margin-left 90px

</style>
