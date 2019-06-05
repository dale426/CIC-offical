<template>
    <div class="page-home">
        <div class="home__banner">
            <div v-swiper:mySwiper="swiperOption">
                <div class="swiper-wrapper">
                    <div class="swiper-slide" v-for="(item, index) in banners" :key="index">
                        <img class="banner__item-img" :src="item.src">
                    </div>
                </div>
                <div class="swiper-button-prev"></div>
                <!--左箭头。如果放置在swiper-container外面，需要自定义样式。-->
                <div class="swiper-button-next"></div>
                <!--右箭头。如果放置在swiper-container外面，需要自定义样式。-->
                <div class="swiper-pagination swiper-pagination-bullets"></div>
            </div>
        </div>
        <section class="home__container">内容区域</section>
    </div>
</template>

<script>
export default {
    layout: 'MainWrap',
    data() {
        return {
            // "path":',
            banners: [{
                id: '1',
                src: 'https://ss3.baidu.com/-fo3dSag_xI4khGko9WTAnF6hhy/image/h%3D300/sign=b5e4c905865494ee982209191df4e0e1/c2cec3fdfc03924590b2a9b58d94a4c27d1e2500.jpg'
            }, {
                src: 'https://ss1.bdstatic.com/70cFvXSh_Q1YnxGkpoWK1HF6hhy/it/u=3501889460,1477116297&fm=26&gp=0.jpg',
                id: 2
            }, {
                src: 'https://cdn.juban.com/BANNER%2F86AD4E1442B17C3E73CDD189820136C4',
                id: 3
            }
            ],
            swiperOption: {
                loop: true, //循环模式
                autoplay: {
                    delay: 3000
                },
                speed: 1000, // 滑动速度
                slidesPerView: 'auto',
                centeredSlides: true,
                spaceBetween: 0, // 轮播图之间的间距
                watchSlidesVisibility: true,
                mousewheel: true, //鼠标滚动
                // 前后导航
                navigation: {
                    nextEl: '.swiper-button-next',
                    prevEl: '.swiper-button-prev',
                },
                pagination: {
                    el: '.swiper-pagination',
                    clickable: true, // 分页器点击
                    dynamicBullets: false // 动态分页器，当你的slide很多时，开启后，分页器小点的数量会部分隐藏。
                },
                controller: true,
                on: {
                    slideChange() {
                        console.log('onSlideChangeEnd', this);
                    },
                    tap() {
                        console.log('onTap', this);
                    }
                },

            }
        }
    },
    mounted() {
        // var mySwiper = new Swiper('.swiper-container', {
        // //controller: true,
        // });
        // setInterval(() => {
        //     console.log('simulate async data')
        //     if (this.swiperSlides.length < 10) {
        //         this.swiperSlides.push(this.swiperSlides.length + 1)
        //     }
        // }, 3000)

    },
    components: {

    }
}
</script>

<style lang="less">
.home__banner {
    width: 100%;
    height: 400px;
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
.banner__item-img {
    object-fit: cover;
    height: 400px;
    width: 100%;
}
</style>
