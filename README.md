# css-vertical-centering
CSS实现任意的单行(多行)垂直居中


## CSS
```css
.vcenter {
    position: relative;
    height: 100%;
}
.vcenter-child {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    width: 100%;
    margin: auto;
    display: table;
    text-align: center;
}
```

## HTML
```html
<!-- 我们需要垂直居中的容器 -->
<div class="container">
    <div class="vcenter">
        <div class="vcenter-child">vertical-centering, 我要垂直居中</div>
    </div>
</div>
```
