<template lang="html">
    <article class="">
      <Slider :items="items" :cname="$style.slider"/>
      <section :class="$style.list">
        <div :class="$style.item" v-for="item in enters" :key="item.img">
          <router-link :to="{name:item.href}">
            <img :src="item.img" :alt="item.title">
            <h4>{{item.title}}</h4>
          </router-link>
        </div>
      </section>
      <section :class="$style.list">
        <div :class="$style.item" v-for="item in enters" :key="item.img">
          <router-link :to="{name:item.href}">
            <img :src="item.img" :alt="item.title">
            <h4>{{item.title}}</h4>
          </router-link>
        </div>
      </section>
    </article>
</template>

<script>
    import Slider from "../core/slider.vue";
    export default {
      name: "hslider",
      components: {
        Slider,
      },
      data(){
        return{
          items:[{
            href:"home1",
            src:"//img12.360buyimg.com/jrpmobile/jfs/t25759/60/2272607322/48838/438e6aad/5bc6f6a5Ncd00b8cb.jpg?width=750&height=320",
          },{
            href:"home2",
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/4666/5/13746/82184/5bd98633E1d2a7f34/2fd9caf35f9e5a8a.jpg?width=750&height=320",
          },{
            href:"home3",
            src:"//img12.360buyimg.com/jrpmobile/jfs/t1/8154/20/4177/48862/5bd98534E5d9de022/b6dd43ca38fcc9ee.jpg?width=750&height=320",
          }],

          enters:[{
            href:'download',
            img:"//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132",
            title:"优惠券",
          },{
            href:'home4',
            img:"//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132",
            title:"领红包",
          },{
            href:'home5',
            img:"//img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png?width=132&height=132",
            title:"抢钢镚",
          },{
            href:'home6',
            img:"//img12.360buyimg.com/jrpmobile/jfs/t1/520/34/950/3686/5b9239e3Eaaf5465c/8d8c35badacfc114.png?width=90&height=90",
            title:"领京豆",
          },{
            href:'home7',
            img:"//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135",
            title:"白条提额",
          }],
        }
      }
    }
</script>

<style lang="scss" module>
  @import "../assets/css/element.scss";
  .slider{
    margin-top: 120px;
    img{
      width: 100%;
    }
  }
  .list{
    @include list(row);
    background: #fff;
    padding-top: 40px;
    padding-bottom: 20px;
    justify-content:space-around;
    a{
      text-decoration: none;
    }
    .item{
      text-align: center;
      img{
        display: inline-block;
        width: 90px;
        height: 90px;
      }
      h4{
        font-size: 26px;
        margin-top: 12px;
        color: #666;
      }
    }

  }
</style>
