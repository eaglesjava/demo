#滚动视差
---

<div class="wrapper">
    <div class="pages">
        <!-- 第一屏 -->
        <section class="page">
            <div class="box1" data-animation="slideToBottom" data-timing-function="ease-in"></div>
            <div class="box2" data-animation="slideToTop" data-delay="300" data-timing-function="ease-out"></div>
            <div class="box3" data-animation="slideToRight" data-delay="600" data-timing-function="linear"></div>
            <div class="box4" data-animation="slideToLeft" data-delay="900" data-timing-function="cubic-bezier(.12,.73,.62,1.38)"></div>
        </section>
        <!-- 第二屏 -->
        <section class="page">
            <div class="box1" data-animation="followSlide" data-duration="1000"></div>
            <div class="box2" data-animation="followSlide" data-delay="200" data-duration="1000"></div>
            <div class="box3" data-animation="followSlide" data-delay="400" data-duration="1000"></div>
            <div class="box4" data-animation="followSlide" data-delay="600" data-duration="1000"></div>
        </section>
        <!-- 第三屏 -->
        <section class="page">
            <div class="box1" data-animation="fadeInToBottom"></div>
            <div class="box2" data-animation="fadeInToTop" data-delay="200"></div>
            <div class="box3" data-animation="fadeInToLeft" data-delay="400"></div>
            <div class="box4" data-animation="fadeInToRight" data-delay="600"></div>
        </section>
        <!-- 第四屏 -->
        <section class="page">
            <div class="box1" data-animation="fadeIn"></div>
            <div class="box2" data-animation="fadeOut" data-delay="800"></div>
        </section>
    </div>
</div>

<!-- <script src="http://i.gtimg.cn/vipstyle/frozenjs/1.0.0/effect.parallax.js"></script> -->

<script src="frozenjs/1.0.1/effect.parallax.js"></script> 
<script>
$('.pages').parallax({
    arrow: true
});
</script>
