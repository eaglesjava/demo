#轮播组件
--- 
<div class="ui-slider">
    <ul class="ui-slider-content" style="width: 300%">
        <li><span style="background-image:url(http://placehold.sinaapp.com/?640*200)"></span></li>
        <li><span style="background-image:url(http://placehold.sinaapp.com//?640*200)"></span></li>      
        <li><span style="background-image:url(http://placehold.sinaapp.com//?640*200)"></span></li>
    </ul>
</div>
内容

<script>
window.addEventListener('load', function(){

    var slider = new fz.Scroll('.ui-slider', {
        role: 'slider',
        indicator: true,
        autoplay: true,
        interval: 3000
    });

    slider.on('beforeScrollStart', function(fromIndex, toIndex) {
        console.log(fromIndex,toIndex)
    });

    slider.on('scrollEnd', function() {
        console.log('end')
    });
})
</script>
