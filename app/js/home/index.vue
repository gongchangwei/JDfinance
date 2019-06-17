<template>
  <div>
      <Heador/>
      <Slider/>
      <Money/>
			<Reward/>
			<Insurance/>
      <Newproduct/>
      <Footor/>
      <Navbar/>
  </div>
</template>

<script>
import Heador from '../public/header.vue';
import Footor from '../public/footer.vue';
import Navbar from '../public/navbar.vue';
import Slider from './hslider.vue';
import Money from './money.vue';
import Newproduct from './newproduct.vue';
import Reward from './reward.vue';
import Insurance from './insurance';


  export default {
    components:{
      Heador,
      Slider,
      Money,
      Newproduct,
			Reward,
			Insurance,
      Footor,
      Navbar,
    }
  }
</script>

<style lang="scss">
@import '../../css/reset.scss';
  
</style>