<template>
    <Panel title="赏金任务" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.arrow">查看更多任务 &gt;</div>
            <Slider :options="options" :items="items" cname="product-slider"/>        
        </section>
    </Panel>
</template>

<script>
import Panel from '../core/panel.vue';
import Slider from '../core/slider.vue';
    export default {
        components:{
            Panel,
            Slider,
        },
        data() {
            return {
                options: {
                    slidesPerView:2.2,
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
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t27040/190/1395454031/8316/d3d74de2/5bc82eb2N34a7625d.png?width=210&height=260',
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
                height:314px;
            }
        }
    }
}
</style>
<style lang="scss" module>
@import "../../css/element.scss";
.panel{
    @include panel;
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