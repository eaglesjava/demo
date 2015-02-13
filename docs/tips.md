#提示条
---

<div class="ui-tooltips ui-tooltips-warn">
    <div class="ui-tooltips-cnt ui-tooltips-cnt-link ui-border-b">
        <i></i>当前网路不可用，请检查你的网路设置。
    </div>
</div>
<div class="ui-tooltips ui-tooltips-guide">
    <div class="ui-tooltips-cnt ui-border-b">
        新手引导、功能引导
        <button class="ui-btn">加入</button>
    </div>
</div>
<div class="ui-tooltips ui-tooltips-state">
    <div class="ui-tooltips-cnt ui-border-b">
        状态
        <button class="ui-btn ui-btn-primary">加入</button>
    </div>
</div>
<div class="ui-tooltips ui-tooltips-vip">
    <div class="ui-tooltips-cnt">
        <i class="ui-icon-vip"></i>
        <span>QQ会员xxxx</span>
        <button class="ui-btn-vip">开通</button>
    </div>
</div>
<div class="ui-tips ui-tips-info">
    <i></i>提供相关的信息或建议
</div>
<div class="ui-tips ui-tips-warn">
    <i></i>警示已经发生或可能在未来发生的问题
</div>
 <div  class="ui-tips ui-tips-success">
    <i></i>提示操作成功或流程成功
</div>
<div class="ui-tips-news-wrap">
    <div  class="ui-tips-news">
        新消息
    </div>
</div>
<div class="ui-btn-group ui-btn-group-bottom">
    <button type="button" id="btn1">成功提示</button>
    <button type="button"  id="btn2">内容提示</button>
    <button type="button"  id="btn3">警告提示</button>
</div> 
<script type="text/javascript">
var el,el2,el3;
$("#btn1").tap(function(){
    el=$.tips({
        content:'温馨提示内容',
        stayTime:2000,
        type:"success"
    })
    el.on("tips:hide",function(){
        console.log("tips hide");
    })

});
$("#btn2").tap(function(){
    el2=$.tips({
        content:'温馨提示内容',
        stayTime:2000,
        type:"info"
    })
    el2.on("tips:hide",function(){
        console.log("tips hide");
    })
});
$("#btn3").tap(function(){
    el3=$.tips({
        content:'温馨提示内容',
        stayTime:2000,
        type:"warn"
    })
    el3.on("tips:hide",function(){
        console.log("tips hide");
    })
});
</script>
