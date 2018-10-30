<template lang="html">
    <div class="header">
      <span class="left">
        <em>注册</em>&nbsp;|&nbsp;<em>登录</em>
      </span>
      <btn class="right">APP下载</btn>
    </div>
</template>

<script>
    import Btn from "../core/btn.vue";
    export default {
      name: "header",
      components: {
          Btn,
        }
    }
</script>

<style lang="scss">
  .header{
    color:#666;
    height: 100px;
    line-height: 100px;
    position:fixed;
    top: 0;
    left: 0;
    right: 0;
    font-size: 32px;
    background: #ffffff url("//m.jr.jd.com/spe/qyy/main/images/jr-logo.png") center center no-repeat;
    background-size: auto 50%;
    z-index: 100;
  }
</style>
