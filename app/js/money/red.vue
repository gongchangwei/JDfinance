<template lang="html">
	<Panel :class="$style.panel">
	    <router-link :to="{name:'money'}">
	        <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/81581/32/1649/30407/5cff825aEda96d532/3d33b3fc634424dd.png?width=750&height=200" alt="">
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
	margin-bottom: 20px;
}
</style>
