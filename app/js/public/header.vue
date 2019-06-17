<template>
	<Panel :class="$style.panel">
		京东金融
	</Panel>
</template>

<script>
import Panel from '../core/panel.vue'
    export default {
        components:{
            Panel,
        },
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
	.panel{
		>h4{
			display: none;
		}
		float: left;
		padding: 0 140px;
		width: 360px;
		height: 88px;
		line-height: 88px;
		border-bottom: 1px solid #e5e5e5;
		font-size: 32px;
		position:fixed;
		top:0;
		left:0;
		right:0;
		z-index:100;
		text-align: center;
		overflow: hidden;
		-o-text-overflow: ellipsis;
		text-overflow: ellipsis;
		white-space: nowrap;
	}
</style>