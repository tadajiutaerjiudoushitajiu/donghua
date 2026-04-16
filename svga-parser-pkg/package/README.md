# SvgaParser   以后有时间改下，web用lite

1.9.7版本支持web版本解析，包体小，web应用尽量用这个

2.0.0及以后版本同时支持web和微信小程序及淘宝小程序解析
（淘宝小程序使用，链接必须使用阿里系的白名单域名，或者云存储cloud://链接）

单纯将svga文件解析成动画图片及动画数据。

### 网页使用
```html
 <script type="text/javascript" src="../build/svgaParser.min.js"></script>
 <script>
        SvgaParser.loadSvga("./svga/step1-1.svga", (v) => {
            console.log(v)
        }, (err) => { console.log(err) })
    </script>
```


### npm使用
```js
npm install svga-parser
import { loadSvga } from "svga-parser";
loadSvga("./svga/step1-1.svga", (v) => {
    console.log(v)
}, (err) => { console.log(err) })
```

