# message

---

// 消息提示

---

## 演示

<link type="text/css" rel="stylesheet" media="screen" href="src/base.css">
<link type="text/css" rel="stylesheet" media="screen" href="src/message.css">

### Message-提示
````html
<div class="ali-message ali-message-info">
    <div class="ali-message-icon"></div>
    <p>提示信息</p>
    <p>提示信息</p>
    <p>提示信息</p>
    <p>提示信息</p>
</div>
````

### Message-警告
````html
<div class="ali-message ali-message-warn">
    <div class="ali-message-icon"></div>
    <p>提示信息</p>
    <p>提示信息</p>
</div>
````

### Message-失败
````html
<div class="ali-message ali-message-error">
    <div class="ali-message-icon"></div>
    <p>成功信息</p>
</div>
````

### Message-成功
````html
<div class="ali-message ali-message-success">
    <div class="ali-message-icon"></div>
    <p>失败信息</p>
</div>
````

### Message-form-提示
````html
<div class="ali-message ali-message-form ali-message-info">
    <div class="ali-message-icon"></div>
    <p>提示信息</p>
</div>
````

### Message-form-失败
````html
<div class="ali-message ali-message-form ali-message-error">
    <div class="ali-message-icon"></div>
    <p>成功信息</p>
</div>
````

### Message-form-成功
````html
<div class="ali-message ali-message-form ali-message-success">
    <div class="ali-message-icon"></div>
    <p>失败信息</p>
</div>
````



<script type="text/javascript">
window.addEventListener('load', function () {
    var interval = 500, begin = Date.now(), img = new Image(), timer = setTimeout(handler, interval);
    window.removeEventListener('load', arguments.callee);
    img.addEventListener('load', handler, false);
    img.src = 'https://i.alipayobjects.com/e/201305/Q9jNoeIir.gif?t=' + begin;

    function handler() {
        clearTimeout(timer);
        img.removeEventListener('load', handler);
        //响应在500ms以内算高速网络 高清（HD）标清（SD）
        document.body.className = (document.body.className + (Date.now() - begin < interval ? ' ali-hd' : ' ali-sd')).trim();
    }
}, false);
</script>