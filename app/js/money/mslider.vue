<template>
    <article>
        <Slider :items="items" :cname="$style.slider" />
        <section :class="$style.list">
        </section>
    </article>
</template>

<script>
import Slider from '../core/slider.vue';
    export default {
        components:{
            Slider,
        },
        data(){
            return{
                items:[{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/53518/5/2325/49052/5d030e52Ec7acdeca/0d9632ae76e5b1ae.png?width=686&height=396',
                    href:'money'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/46879/19/504/107897/5cdea0baE7a0eaf0c/d4db650be0adb4d4.png?width=750&height=400',
                    // href:'money'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t1/31588/6/14705/52443/5cbeb2b2Ea0648bba/e05f04db25d47126.png?width=750&height=400',
                    // href:'money'
                },{
					src:'//img12.360buyimg.com/jrpmobile/jfs/t1/39579/28/7701/58742/5cedf514E09a23a3f/e56192beb56f80f3.jpg?width=750&height=400',
					// href:'money'
				},{
					src:'//img12.360buyimg.com/jrpmobile/jfs/t1/38925/1/7734/32802/5cef91cfE8962dc90/08a7df363c6465f2.png?width=750&height=400',
					// href:'money'
				}]
            }
        }
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
.slider{
    margin:90px 0 20px;
    img{
        width:100%;
    }
}
section{
    background-color:#fff;
}
</style>