<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <swiper-slide v-for="item of swiperList" :key="item.id">
                <img class="swiper-img" :src="item.imgUrl" />
            </swiper-slide>
           
            <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </div>
    
</template>
<script>
    export default{
        name:'HomeSwiper',
        data (){
            return{
                swiperOption:{
                    pagination:'.swiper-pagination'
                },
                swiperList:[{
                    id:'0001',
                    imgUrl:'http://img1.qunarzz.com/piao/fusion/1807/5e/cfee2e9e2f357202.jpg_750x200_b0308a43.jpg'
                },{
                    id:'0002',
                    imgUrl:'http://img1.qunarzz.com/piao/fusion/1809/2b/c25da1803eb25502.jpg_750x200_e42fe8ee.jpg'
                }]
            }
        }
    }
</script>
<style lang="stylus" scoped>
    .wrapper >>> .swiper-pagination-bullet .swiper-pagination-bullet-active
        background: #fff !important
    .wrapper
        overflow:hidden
        width:100%
        height:0
        padding-bottom:31.25%
        .swiper-img
            width:100%
</style>