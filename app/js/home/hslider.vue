<template>
    <article>
        <!-- <Slider :items="items" :cname="$style.slider" /> -->
        <section :class="$style.list">
            <div :class="$style.item" v-for="item in enters" :key="item.img">
                <router-link :to="{name:item.href}">
                    <img :src="item.img" alt="">
                </router-link>
                <h4>{{item.title}}</h4>
            </div>
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
                /* items:[{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t16213/283/2014672290/33503/a5e64858/5a785d99N5cd3136f.jpg?width=750&height=320',
                    herf:'https://storage.jd.com/bk.jd.com/static/m/bcm_act.html?applyChannel=MOBILE-OPEN2&sid=&qingfrom=pcurl/?from=jrad_1830098'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t14554/107/2216340839/36640/ecbf2d05/5a785d72Nec40e2bb.jpg?width=750&height=320',
                    href:'home'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t19342/207/437037473/41615/a77ec600/5a785db6N33b8cc7d.jpg?width=750&height=320',
                    href:'home'
                },{
                    src:'//img12.360buyimg.com/jrpmobile/jfs/t16486/292/2052342436/22366/2af9a69d/5a785dd3Nb5e10fbd.jpg?width=750&height=320',
                    href:'home' 
                }], */                
                enters:[{
                    img:'//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
                    href:'',
                    title:'优惠劵',
                },{
                    img:'//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132',
                    href:'home',
                    title:'领福利'
                },{
                    img:'//img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png?width=132&height=132',
                    href:'home',
                    title:'抢钢镚'
                },
                // {
                //     img:'//img12.360buyimg.com/jrpmobile/jfs/t4618/115/2179710654/11347/bf520df/58ec9d84Nfd169001.png?width=132&height=132',
                //     href:'home',
                //     title:'领京豆'
                // },
                {
                    img:'//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135',
                    href:'download',
                    title:'白条提醒'
                },{
                    img:'//img12.360buyimg.com/jrpmobile/jfs/t1/520/34/950/3686/5b9239e3Eaaf5465c/8d8c35badacfc114.png?width=90&height=90',
                    href:'home',
                    title:'工资理财'
                },{
                    img:'//img12.360buyimg.com/jrpmobile/jfs/t1/1216/39/659/4516/5b923b1cE5943d1c6/dabaf8b842f57eb9.png?width=90&height=90',
                    href:'home',
                    title:'众筹'
                },{
                    img:'//img12.360buyimg.com/jrpmobile/jfs/t1/36242/13/119/12214/5cb06492E0c73a66f/a284f91242e27af1.png?width=90&height=90',
                    href:'home',
                    title:'免费领京豆'
                },{
                    img:'//img12.360buyimg.com/jrpmobile/jfs/t1/23337/6/15445/8974/5cb064c2E0cadac1d/c533bfe4da578fe7.png?width=90&height=90',
                    href:'home',
                    title:'免息红包'
                }]
            }
        }
    }
</script>

<style lang="scss" module>
@import '../../css/element.scss';
/* .slider{
    margin-top:120px;
    img{
        width:100%;
    }
} */
.list{
    @include list(row);
	margin-top: 90px;
    padding-top:40px;
    padding-bottom:20px;
    justify-content:space-around;
    background-color:#fff;
    .item{
        text-align:center;
		width:25%;
		padding-bottom:40px;
        a{
			text-decoration:none;
        }
        img{
			display: inline-block;
            width:90px;
            height:90px;
        }
        h4{
           font-size:26px;
           color:#666;
           margin-top:12px;
           white-space:nowrap;
           text-overflow:ellipsis; 
           overflow:hidden;
        }
    }
}
</style>