<template>
    <Panel title="众筹新品" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.arrow">更多尖货 &gt;</div>
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
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/30149/40/8970/20149/5ca2e84dE7641a4dc/342b926b8582a140.jpg?width=335&height=421',
                    href:'1'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/19514/33/13824/16597/5ca2e84eE4b9cc39a/23b319b8846b585c.png?width=335&height=421',
                    href:'2'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/12202/17/13916/19329/5ca2e84fE6bde713f/ff4f3231eb4c7312.jpg?width=335&height=421',
                    href:'3'
                }/* ,{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t19438/256/457591773/38627/1f0fb065/5a7d5bd0N656c015c.jpg?width=335&height=421',
                    href:'4'
                } */]
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