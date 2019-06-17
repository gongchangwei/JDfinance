<template>
    <Panel2 title="赏金任务" more="查看更多任务" :class="$style.panel2">
        <section :class="$style.content">
			<Slider :options="options" :items="items" cname="product-slider"/>
        </section>
    </Panel2>
</template>

<script>
import Panel2 from '../core/panel2.vue';
import Slider from '../core/slider.vue';
    export default {
        components:{
            Panel2,
            Slider,
        },
        data() {
            return {
                options: {
                    slidesPerView:2.7,
                    spaceBetween: 24,
                    freeMode: true
                },
                items:[{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t26893/316/1416172900/5740/58f20b1e/5bc82e3aN7aa90a89.png?width=210&height=260',
                    href:'1'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t26767/72/1365822552/8516/2e071d95/5bc82e6eN0be93809.png?width=210&height=260',
                    href:'2'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t30418/166/1039421072/8983/a6f90d5b/5c04eccbN581f6287.png?width=210&height=260',
                    href:'3'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t26182/297/1417522782/7864/19181a3b/5bc82ec0N0824153d.png?width=210&height=260',
                    href:'4'
                }]
            }
        }
    }
</script>
<style lang="scss">
.product-slider {
    .swiper-container{
        padding:0 24px;
        .swiper-slide{
            img{
                width:100%;
                height:260px;
				background:#eee;
            }
        }
    }
}
</style>
<style lang="scss" module>
@import "../../css/element.scss";
.panel{
    @include panel2;
    .content{
        position:relative;
        padding-bottom:24px;
        .arrow{
            position:absolute;
            top:-78px;
            right:32px;
            font-size:28px;
            color:#999;
        }
    }
}
</style>