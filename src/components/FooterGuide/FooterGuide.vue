<template>
    <div class="footer_guide">
        <div class="guide">
            <div class="guide_items" :class="{on: '/msite' === $route.path}" @click="goTo('/msite')">
                <span>img</span>
                <p>外卖</p>
            </div>

            <div class="guide_items" :class="{on: '/search' === $route.path}" @click="goTo('/search')">
                <span>img</span>
                <p>搜索</p>
            </div>

            <div class="guide_items" :class="{on: '/order' === $route.path}" @click="goTo('/order')">
                <span>img</span>
                <p>订单</p>
            </div>

            <div class="guide_items" :class="{on: '/profile' === $route.path}" @click="goTo('/profile')">
                <span>img</span>
                <p>我的</p>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name:"FooterGuide",
    methods:{
        goTo(path) {
            this.$router.replace(path);
            console.log(this.$route.path)
        }
    }
}
</script>

<style lang="stylus">
@import "../../common/stylus/mixins.styl"
.footer_guide
    position fixed
    width 100%
    height 50
    bottom: 0
    left: 0
    background-color: #e4e4e4
    .guide
        display flex
        justify-content space-around
        align-content center
        .guide_items
            color: blue
</style>