# 基于sspanelv3mod
弹框功能
尽量使用notepad等软件编辑

必须！   在user数据库加一个int字段 displayan  不能为空 默认为0

1.在/www/wwwroot/ssr/resources/views/material/user/下的页面 加入下列 后续自行修改内容 
<script>
   $(document).ready(function () {
  
   if({$user->displayan}== "1"){
      $("#result").modal();
	$("#msg").html("<p>愚人节PY码8折(目前可用) : <b>500811<b></p><h4>谢谢支持！！！<p>如需取消弹框请在左侧资料编辑设置</p></h4>");
     }else{}
  
  })
</script>

2.将edit.tpl替换掉 /www/wwwroot/ssr/resources/views/material/user/下
  将routes.php替换/www/wwwroot/ssr/config/下
  将UserController.php替换 /www/wwwroot/ssr/app/Controllers/下
  
  
