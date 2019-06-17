<template>
    <section :class="[panelClass,cname]">
        <h4>{{title}}</h4>
		<h5>{{more}}></h5>
        <slot/>
    </section>
</template>
<script>
    export default {
        props:{
            title:{
                type:String,
                default:''
            },
			more:{
				type:String,
				default:''
			},
            cname:{
                type:String,
                default:''
            }
        },
        data(){
           return{
               panelClass:'panel2'
           }
        } 
    }
</script>
<style lang="scss">
@import '../../css/element.scss';
.panel2{
    @include panel2;
}   
</style>