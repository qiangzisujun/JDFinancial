<template lang="html">
  <Panel title="极速借贷" :class="$style.panel">
    <section :class="$style.content">
      <router-link :to="{name:'home',params:{}}">
        <img src="//img12.360buyimg.com/jrpmobile/jfs/t25759/60/2272607322/48838/438e6aad/5bc6f6a5Ncd00b8cb.jpg?width=750&height=320" alt="">
      </router-link>
    </section>
  </Panel>
</template>

<script>
    import Panel from "../core/panel";
    export default {
        name: "borrow",
        components: {Panel}
    }
</script>

<style lang="scss" module>
  @import "../assets/css/element.scss";
  .panel{
    @include panel;
    .content{
      padding-bottom: 40px;
      img{
        display: block;
        width: 100%;
      }
    }
  }
</style>
