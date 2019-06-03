<template>
    <div class="page-home">
        <div class="home__banner">预留banner位置</div>
        <section class="home__container">内容区域</section>
    </div>
</template>

<script>

export default {
    layout: 'main',
    components: {
    }
}
</script>

<style lang="less">
.page-home {
}
.home__banner {
    width: 100%;
    height: 300px;
    border: 2px dotted blue;
}
.home__container {
    border: 1px solid red;
    margin: 0 auto;
    display: flex;
    width: 1200px;
    justify-content: center;
    align-items: center;
    text-align: center;
}
</style>
