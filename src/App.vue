<template lang="html">
  <div>
    <Herdor/>
    <Slider/>
    <Novice/>
    <Borrow/>
    <Money/>
    <Product/>
    <Life/>
    <Footer/>
    <Navbar/>
  </div>
</template>

<script>
  import Herdor from "@/public/header"
  import Slider from "@/home/hslider"
  import Novice from "@/home/novice";
  import Borrow from "@/home/borrow";
  import Money from "@/home/money";
  import Product from "./home/product";
  import Life from "./home/life";
  import Footer from "./public/footer";
  import Navbar from "./public/navbar";

  export default {
    components:{
      Navbar,
      Footer,
      Life,
      Product,
      Money,
      Borrow,
      Herdor,
      Slider,
      Novice,
    }
  }
</script>

<style scoped>

</style>
