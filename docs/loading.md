#加载中 
--- 
<section class="ui-notice">
    <p>加载中...</p>
</section>
<div class="ui-notice-warn">
    <i class="ui-icon ui-icon-refresh loading"></i><p>请检查网络</p>
</div>
<div class="ui-loading-wrap">
    <p>加载中</p>
    <i class="ui-loading"></i>
</div>

<div class="ui-center">
    <div class="ui-btn" id="btn1">弹出loading</div>
</div>

<script type="text/javascript">
$("#btn1").tap(function(){
    var el=$.loading({
        content:'加载中...',
    })
    setTimeout(function(){
        el.loading("hide");
    },2000);
    el.on("loading:hide",function(){
        console.log("loading hide");
    });
});
</script>