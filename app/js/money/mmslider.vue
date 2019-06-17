<template lang="html">
	<article class="">
		<section :class="$style.list">
			<div :class="$style.item" v-for="item in enters" :key="item.img">
				<router-link :to="{ name: item.href}">
					<img :src="item.img" alt="item.title">
					<h4>{{item.title}}</h4>
				</router-link>
			</div>
		</section>
	</article>
</template>

<script>
	import Slider from "../core/slider.vue"
	export default {
		components: {
			Slider,
		},
		data(){
			return {
				items:[],
				enters: [{
					href: "money",
					img: "//img12.360buyimg.com/jrpmobile/jfs/t1/84319/32/1755/3025/5d020d8cE7666fc33/8d2bb6cd9142917a.png?width=90&height=90",
					title: "抢免单",
				},{
					href: "money",
					img: "//img12.360buyimg.com/jrpmobile/jfs/t1/22708/8/15082/7446/5cad5c35E7e3ae22b/72adc577175d7c4f.png?width=90&height=90",
					title: "双签",
				},{
					href: "money",
					img: "//img12.360buyimg.com/jrpmobile/jfs/t1/62829/35/1167/4169/5cf64e75Ec0e5b729/eb07348c21179775.png?width=90&height=90",
					title: "优惠券",
				},{
					href: "money",
					img: "//img12.360buyimg.com/jrpmobile/jfs/t1/47642/31/1640/4856/5cf64f24E67912a6f/2a4bf9dc9793872b.png?width=90&height=90",
					title: "单单返京豆",
				},{
					href: "money",
					img: "//img12.360buyimg.com/jrpmobile/jfs/t29131/288/288291507/3943/bed46aef/5bee6bd5Nfc5d5360.png?width=90&height=90",
					title: "全部",
				}],
			}
		},
	}
</script>

<style lang="scss" module>
	@import "../../css/element.scss";
	.list{
		@include list(row);
		background: #fff;
		justify-content: space-around;
		a{
			text-decoration: none;
		}
		.item{
			text-align: center;
			width: 20%;
			img{
				display: inline-block;
				width: 90px;
				height: 90px;
				margin: 38px 19px 0;
			}
			h4{
				font-size: 24px;
				margin-top: 18px;
				margin-bottom:48px;
				color: #333;
			}
		}
	}
</style>
