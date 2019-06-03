<template>
    <div class="page-home">
        <div class="home__banner">预留banner位置</div>
        <section class="container">内容区域</section>
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
.container {
    border: 1px solid red;
    margin: 0 auto;
    /* min-height: 100vh; */
    display: flex;
    width: 1200px;
    justify-content: center;
    align-items: center;
    text-align: center;
}
</style>
