<template lang="html">
	<Panel :class="$style.panel">
	    <router-link :to="{name:'money'}">
	        <img src="//img12.360buyimg.com/jrpmobile/jfs/t20746/93/1719082958/12040/306a2296/5b31b40dNeefe4c3c.png?width=750&height=200" alt="">
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
	padding: 20px 0 40px;
}
</style>
