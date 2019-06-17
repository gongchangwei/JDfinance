<template lang="html">
	<Panel :class="$style.panel">
	    <router-link :to="{name:'money'}">
	        <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/37697/16/1334/187953/5cb44c65E5dbefe83/200ce71a4347aeec.png?width=750&height=200" alt="">
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
	padding: 0 0 40px;
	margin: 0 0 20px;
}
</style>
