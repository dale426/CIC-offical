<template>
    <div class="layout__main">
        <div class="layout__main-wraps">
            <div class="layout__main-title">
                <img class="logo" :src="cic_logo" alt="logo">
                <span>中以西北国际科技创新中心</span>
            </div>
            <menu class="layout__menu-wrap clearfix" type="list">
                <li class="layout__menu-item">
                    <a href="/">
                        <i class="icon-menu iconfont icon-homepage"></i>首页
                    </a>
                </li>
                <li class="layout__menu-item">
                    <a href="/cic/technology">
                        <i class="icon-menu iconfont icon-homepage"></i>技术包发布
                    </a>
                </li>
                <li class="layout__menu-item">
                    <a href="/cic/innovate">
                        <i class="icon-menu iconfont icon-homepage"></i>创新前沿
                    </a>
                </li>
                <li class="layout__menu-item">
                    <a href="/cic/club">
                        <i class="icon-menu iconfont icon-homepage"></i>六芒星俱乐部
                    </a>
                </li>
                <li class="layout__menu-item">
                    <a href="/cic/news">
                        <i class="icon-menu iconfont icon-homepage"></i>新闻聚焦
                    </a>
                </li>
                <li class="layout__menu-item">
                    <a href="/cic/concat">
                        <i class="icon-menu iconfont icon-homepage"></i>联系我们
                    </a>
                </li>
            </menu>
        </div>
        <nuxt/>
    </div>
</template>
<script>
import logo from '~/assets/img/logo@2x.png'
export default {
    name: 'layout_main',
    data() {
        return {
            cic_logo: logo
        }
    },

}
</script>
<style lang="less">
@import "./main.less";
</style>

