<template>
    <div :class="[wrapClass]"></div>
</template>

<script>
    export default {
        data(){
            return{
                wrapClass:'wrap',
            }
        }
    }
</script>

<style lang="scss">
@import '../../css/element.scss';
.wrap{
    @include wrap;
}
</style>