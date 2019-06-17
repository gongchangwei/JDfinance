<template>
  <div>
      <Heador/>
      <Slider/>
			<Sign/>
			<Mslider/>
			<Go/>
			<Red/>
			<Assignment/>
			<Day30/>
			<Member/>
			<Bank/>
			<Issue/>
			<Contact/>
      <Footor/>
      <Navbar/>
  </div>
</template>

<script>
import Heador from '../public/header.vue';
import Footor from '../public/footer.vue';
import Navbar from '../public/navbar.vue';
import Slider from './mslider.vue';
import Sign from './sign.vue';
import Mslider from './mmslider.vue';
import Go from './go.vue';
import Red from './red.vue';
import Assignment from './assignment.vue';
import Day30 from './day30.vue';
import Member from './member.vue';
import Bank from './bank.vue';
import Issue from './issue.vue';
import Contact from './contact.vue';
  export default {
    components:{
      Heador,
      Slider,
			Sign,
			Mslider,
			Go,
			Red,
			Assignment,
			Day30,
			Member,
			Bank,
			Issue,
			Contact,
      Footor,
      Navbar,
    }
  }
</script>

<style lang="scss">
@import '../../css/reset.scss';
  
</style>