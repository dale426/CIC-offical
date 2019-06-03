<template>
    <div class="layout__main">
        <div class="layout__main-menu">
            <menu class="menu clearfix" type="list">
                <li class="menu-item">
                    <a href="#/home">
                        <i class="icon-menu iconfont icon-homepage"></i>首页
                    </a>
                </li>
                <li class="menu-item">
                    <a href="#/pages1">
                        <i class="icon-menu iconfont icon-homepage"></i>pages1
                    </a>
                </li>
                <li class="menu-item">
                    <a href="/pages1">
                        <i class="icon-menu iconfont icon-homepage"></i>pages1
                    </a>
                </li>
                <li class="menu-item">
                    <a href="/pages1">
                        <i class="icon-menu iconfont icon-homepage"></i>pages1
                    </a>
                </li>
            </menu>
        </div>
        <nuxt/>
    </div>
</template>
<script>
export default {
    name: 'layout_main',

}
</script>
<style lang="less">
@import "./main.less";
</style>

