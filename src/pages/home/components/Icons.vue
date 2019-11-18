<template>
  <div class="icons">
    <swiper>
      <swiper-slide>
        <div class="icon" v-for="item of iconList" :key="item.id">
          <div class="icon-img">
            <img class="icon-img-content" :src='item.imgURL'/>
          </div>
          <p class="icons-desc">{{item.desc}}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>
<script>
export default {
  name: 'HomeIcons',
  data () {
    return {
      iconList: [{
        id: '01',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
        desc: '景点门票'
      }, {
        id: '02',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
        desc: '深圳必游'
      }, {
        id: '03',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/4d/a1eda1a2b8414302.png',
        desc: '夜场狂晃'
      }, {
        id: '04',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/50/26ffa31b56646402.png',
        desc: '海洋馆'
      }, {
        id: '05',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/ab/6f7d6e44963c9302.png',
        desc: '泡温泉'
      }, {
        id: '06',
        imgURL: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20194/cba147cf6cfcea7109d0bff6aac6f626.png',
        desc: '深圳动物园'
      }, {
        id: '07',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/a6/6d97515091789602.png',
        desc: '世界之窗'
      }, {
        id: '08',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/b6/37560ece9c62b502.png',
        desc: '东部华侨城'
      }, {
        id: '09',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',
        desc: '一日游'
      }, {
        id: '10',
        imgURL: 'http://img1.qunarzz.com/piao/fusion/1803/b1/528a9e80403b8c02.png',
        desc: '玩转长隆'
      }]
    }
  }
}
</script>
<style lang="stylus" scoped>
  @import "~styles/varibles.styl"
    .icons >>> .swiper-container
      overflow: hidden
      height: 0
      padding-bottom: 50%
    .icon
      position: relative
      overflow: hidden
      float: left
      width: 25%
      height: 0
      padding-bottom: 25%

      .icon-img
        position: absolute
        top: 0
        left: 0
        right: 0
        bottom: .44rem
        box-sizing: border-box
        padding: .1rem

        .icon-img-content
          display: block
          margin: 0 auto
          height: 100%

      .icons-desc
        position: absolute
        left: 0
        bottom: 0
        right: 0
        height: .44rem
        line-height: .44rem
        text-align: center
        color: $darkTextColor
</style>
