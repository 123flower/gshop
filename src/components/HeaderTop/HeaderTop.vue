<template>

    <header class="header_top">
        <slot name="left"></slot>
        <span>
            <span>{{title}}</span>
        </span>
        <slot name="right"></slot>
    </header>
       
</template>

<script>

export default {
    name:'HeaderTop',
    props:{
        title:String,
    },

}
</script>

<style lang="stylus">
@import "../../common/stylus/mixins.styl"
.header_top 
    top 0
    left 0
    z-index 100

</style>

