#弹窗
--- 

<div class="ui-center">
    <div class="ui-btn" id="btn1">模板创建弹窗</div>
    <div class="ui-btn" id="btn2">DOM创建弹窗</div>
</div>
<div class="ui-dialog">
    <div class="ui-dialog-cnt">
        <div class="ui-dialog-bd">
            <div>
            <h4>标题</h4>
            <div>内容</div></div>
        </div>
        <div class="ui-dialog-ft ui-btn-group">
            <button type="button" data-role="button"  class="select" id="dialogButton<%=i%>">关闭</button> 
        </div>
    </div>        
</div>
<script type="text/javascript">
$("#btn1").tap(function(){
    var dia=$.dialog({
        title:'温馨提示',
        content:'温馨提示内容',
        button:["确认","取消"]
    });

    dia.on("dialog:action",function(e){
        console.log(e.index)
    });
    dia.on("dialog:hide",function(e){
        console.log("dialog hide")
    });
})
$("#btn2").tap(function(){
    $(".ui-dialog").dialog("show");
})
</script>
