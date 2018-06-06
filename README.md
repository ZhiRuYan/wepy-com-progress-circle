
# 微信小程序wepy的第三方组件：圆形进度条

![](http://oxk008h6r.bkt.clouddn.com/demo.png)

## 说明

官方支持的进度条只有条形进度条，没有圆形进度条，因此增加了一个圆形进度条。
此组件是wepy的第三方组件，因为需要依赖[wepyjs](https://github.com/Tencent/wepy)

## 使用

### 安装组件

```shell
npm install wepy-com-progress-circle --save
```

### 使用组件

```javascript
// index.wpy
<template>
    <progressCircle :percent="percent" width="120" />
</template>
<script>
    import wepy from 'wepy';
    import ProgressCircle from 'wepy-com-progress-circle';

    export default class Index extends wepy.page {
        components = {
            progresscircle: ProgressCircle
        };
        data = {
          percent: 25, 
        }
    }
</script>
```

## API说明

<table>
    <thead>
        <tr>
            <th>属性名</th><th>类型</th><th>默认值</th><th>说明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>width</td><td>Number</td><td>100</td><td>圆的宽度</td>
        </tr>
        <tr>
            <td>showInfo</td><td>Boolean</td><td>true</td><td>在进度条右侧显示百分比</td>
        </tr>
        <tr>
            <td>strokeWidth</td><td>Number</td><td>6</td><td>进度条线的宽度，单位px</td>
        </tr>
        <tr>
            <td>color</td><td>Color</td><td>#09BB07</td><td>进度条颜色</td>
        </tr>
        <tr>
            <td>backgroundColor</td><td>Color</td><td>#eee</td><td>进度条背色颜色</td>
        </tr>
    </tbody>
</talbe>
                                                 	             
