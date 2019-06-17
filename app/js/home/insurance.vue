<template>
    <Panel title="保险保障" :class="$style.panel">
        <section :class="$style.content">
            <div :class="$style.arrow"></div>
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
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/19965/4/1946/28370/5c18958aE9e8a930d/9810bed7979e6bd5.jpg?width=210&height=260',
                    href:'1'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/27283/39/2034/26756/5c1895b5Ecbfdf7ed/6a0755f1f40e2eb9.jpg?width=210&height=260',
                    href:'2'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/27014/35/2022/24897/5c1895d9Ef095679a/c0918d244bbfb2e5.jpg?width=210&height=260',
                    href:'3'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/19150/30/2037/31576/5c1895f2Eb431149e/7a71e063250f8b0d.jpg?width=210&height=260',
                    href:'4'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/9279/3/9618/27165/5c189693E5d54e2cb/c263629839992767.jpg?width=210&height=260',
                    href:'5'
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