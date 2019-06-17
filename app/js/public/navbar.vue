<template>
    <Panel :class="$style.panel">
        <ul :class="$style.content">
            <li>
                <router-link :to="{name:'home'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/8325/8/4331/3095/5bda5c89E1be47c14/47b6a296683a12a5.png?width=90&height=90" alt="">
                    <h4>首页</h4>
                </router-link>
            </li>
            <li>
                <router-link :to="{name:'money'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/1890/15/14183/1269/5bda5c97E34734b01/241a0f5b17fd3e51.png?width=60&height=60" alt="">
                    <h4>赚钱</h4>
                </router-link>
            </li>
            <li>
                <router-link :to="{name:'ious'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/5291/40/14133/594/5bda5ca3E92d0e800/09ac81fa5a5c96ef.png?width=60&height=60" alt="">
                    <h4>借钱</h4>
                </router-link>
            </li>
            <li>
                <router-link :to="{name:'raise'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/3358/38/14064/816/5bda5cabEcb7eca8b/9bb064f1cda7ceba.png?width=60&height=60" alt="">
                    <h4>省钱</h4>
                </router-link>
            </li>
            <li>
                <router-link :to="{name:'home'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/7491/15/4277/926/5bda5cb9E421a0e60/89ee14ce9daf4aab.png?width=60&height=60" alt="">
                    <h4>会员</h4>
                </router-link>
            </li>
        </ul>
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
    position:fixed;
    bottom:0;
    left:0;
    right:0;
	background-color: #fff;
	z-index: 200;
    >h4{
        display:none;
    }
    .content{
        @include flex(row);
        justify-content:space-around;
        height:100px;
        li{
            a{
                text-decoration:none;
            }
            img{
                width:44px;
                height:44px;
                margin:12px auto 6px;
            }
            h4{
                font-size:22px;
                color:#656565;
            }
        }
    }
}
</style>