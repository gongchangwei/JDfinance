<template>
    <Panel2 title="白条" more="年轻不留白" :class="$style.panel2">
        <section :class="$style.content">
			<div :class="$style.xiaobai">
				<Wrap :class="$style.wrap"></Wrap>
			</div>
			<div :class="$style.icosix">
				<Wrap :class="$style.wrap"></Wrap>
			</div>
        </section>
    </Panel2>
</template>

<script>
import Panel2 from '../core/panel2.vue';
import Wrap from '../core/wrap.vue';
    export default {
        components:{
            Panel2,
			Wrap,
        },
        data() {
            return {
                options: {
                    slidesPerView:2.7,
                    spaceBetween: 24,
                    freeMode: true
                },
                items:[{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t11146/24/2920754736/6944/5845636d/5cdd0a6eN9927ae25.png?width=210&height=260',
                    href:'1'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t11293/128/3052512266/21236/ff9211a7/5cde1a7bNec04b900.png?width=210&height=260',
                    href:'2'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/78161/22/1122/6862/5cf64f57E22d73ec6/6db7f006167ae90c.png?width=210&height=260',
                    href:'3'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/52696/34/1660/7438/5cf64f6aE85f1676e/bded5460995cc76e.png?width=210&height=260',
                    href:'4'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t26410/345/1052784155/8412/66e542af/5bc04992N0d13e713.jpg?width=210&height=260',
                    href:'5'
                }]
            }
        }
    }
</script>

<style lang="scss" module>
@import "../../css/element.scss";
.panel2{
    @include panel2;
    .content{
        position:relative;
        padding-bottom:24px;
		width: 640px;
		height: 260px;
		.xiaobai{
			float: left;
			color: #fff;
			padding: 0 16px 0 30px;
			width: 256px;
			height: 260px;
			box-sizing: border-box;
			z-index: 2;
			border-radius: 4px;
			margin-bottom: 16px;
			display: block;
			.wrap{
				@include wrap;
			}
		}
		.icosix{
			float: right;
			padding: 0 30px 0 0;
			width: 384px;
			height: 260px;
			position: relative;
			box-sizing: border-box;
			z-index: 2;
			border-radius: 4px;
			display: block;
			.wrap{
				@include wrap;
			}
		}
    }
}
</style>