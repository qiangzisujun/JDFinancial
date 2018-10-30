<template>
    <section class="cname">
        <swiper :options="options" :not-next-tick="options.notNextTick">
          <swiper-slide>aaaa</swiper-slide>
        </swiper>
    </section>
</template>

<script>
  import { swiper, swiperSlide } from "vue-awesome-swiper"
  export default {
        name: "slider",
        components:{
          swiper,
          swiperSlide,
        },
        props:{
          options:{
            type:Object,
            default(){
              return{
                autoplay:true,
                loop:true,
                pagination:{
                  el:".swiper-pagination",
                },
                notNextTick:false,
              }
            }
          }
        }
    }
</script>

<style lang="scss">
  @import "~swiper/dist/css/swiper.css";
</style>
