<template lang="html">
	<Panel :class="$style.panel">
	    <router-link :to="{name:'money'}">
	        <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/51266/37/2318/54448/5d030e3aE7a4485ab/37fa1ca1be2185df.jpg?width=750&height=200" alt="">
	    </router-link>
	</Panel>
</template>

<script>
import Panel from '../core/panel.vue';
	export default {
		components:{
			Panel,
		},
	}
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.panel{
    @include panel;
	h4{
		display: none;
	}
    img{
        width:100%;
        height:auto;
    }
	padding-bottom: 40px;
}
</style>
