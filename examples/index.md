# Demo

---

````html
<div class="pubuliu-box">
    <div class="img-box">
        <div class="img-inner">
            <img src="images/1.jpg" alt="picture"/>
        </div>
    </div>
    <div class="img-box">
        <div class="img-inner">
            <img src="images/2.jpg" alt="picture"/>
        </div>
    </div>
    <div class="img-box">
        <div class="img-inner">
            <img src="images/3.jpg" alt="picture"/>
        </div>
    </div>
    <div class="img-box">
        <div class="img-inner">
            <img src="images/4.jpg" alt="picture"/>
        </div>
    </div>
    <div class="img-box">
        <div class="img-inner">
            <img src="images/5.jpg" alt="picture"/>
        </div>
    </div>
</div>
````

````css
.pubuliu-box {
  position: relative;
  margin: 0 auto;
}
.pubuliu-box > .img-box {
  float: left;
  padding: 5px;
}
.pubuliu-box > .img-box > .img-inner {
  border: 1px solid #cccccc;
  padding: 5px;
  border-radius: 5px;
  -webkit-box-shadow: 0 0 5px #ccc;
  -moz-box-shadow: 0 0 5px #ccc;
  box-shadow: 0 0 5px #ccc;
}
.pubuliu-box > .img-box > .img-inner > img {
  display: block;
  width: 150px;
  height: auto;
}
````

````javascript
var movingWater = require('moving-water');
movingWater.init('.pubuliu-box','.img-box',function(parent){
    console.log('当滚动条往下拉，拉动到显示完最后一张图片时，回调要干的事');
});
````

