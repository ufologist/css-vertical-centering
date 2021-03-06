# css-vertical-centering
CSS实现任意的单行(多行)垂直居中

## 这种方式实现的垂直居中灵活在哪里?
* 不需要知道待垂直居中的容器高度(意味着不需要写死任何高度数值)
* 支持多行垂直居中
* 可做为工具样式来使用, 例如这里的: ```.vcenter```, ```.vcenter-child```

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

## Demo
[vertical-centering](http://ufologist.github.io/css-vertical-centering/vertical-centering.html)
