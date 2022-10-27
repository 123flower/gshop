<template>
    <div>
        <HeaderTop :title="address.name"></HeaderTop>
        Msite
        
    </div>
</template>

<script>
import HeaderTop from '../../components/HeaderTop/HeaderTop.vue';
import { mapState } from 'vuex';

export default {
    name:"Msite",
    components:{
        HeaderTop,
    },
    computed:{
        ...mapState(['address'])
    },
}
</script>

<style lang="stylus" >

</style>