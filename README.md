# moving-water [![spm version](http://spmjs.io/badge/moving-water)](http://spmjs.io/package/moving-water)

---

布瀑流图片展示效果

## Install

```
$ spm install moving-water --save
```

## Usage

```js
var movingWater = require('moving-water');
// use movingWater.init(parent,child,callback);
```
## 介绍

这个模块用于布瀑流图片展示效果

这个模块对象暴露了一个init方法，有三个参数：movingWater.init(parent,child,callback);

- parent : 包裹图片元素的布局元素的引用,即下边html结构对应的pubuliu-box

html结构如下

```html
<div class="pubuliu-box">
    <div class="img-box">
        <div class="img-inner">
            <img src="images/1.jpg" alt="picture"/>
        </div>
    </div>
    <div class="img-box">...</div>
    ...
</div>    
```

- child ：包裹图片元素的引用，即上边html结构对应的img-box
- callback : 当滚动条往下拉，拉动到显示完最后一张图片时，回调要干的事

