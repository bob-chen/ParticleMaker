# ParticleMaker
Canvas 粒子动画

支持使用图片或文字做粒子动画。

支持普通使用，AMD，CMD。

### 使用方法：

使用文字：

```javascript

    var particleMaker = new ParticleMaker({
         canvasId: "canvas",
         startX: 200,
        startY: 400,
        endX: 10,
        endY: 40,
        content: "Test",
        fillColor: "#ff4444",
        effect: "easeOutQuad",
        onFinish: function(){
            console.log("onFinish");
            console.log(l);
           }
   });
   particleMaker.run();
```

使用图片

```javascript

    l = new Image();
    l.src = "images.jpeg";

    var particleMaker = new ParticleMaker({
         canvasId: "canvas",
         startX: 200,
        startY: 400,
        endX: 10,
        endY: 40,
        content: l,
        fillColor: "#ff4444",
        effect: "easeOutQuad",
        onFinish: function(){
            console.log("onFinish");
            console.log(l);
           }
   });
   particleMaker.run();
```

### 效果

![http://ww3.sinaimg.cn/large/0060lm7Tgw1f8hqbgormlg30cs0fuh4t.gif](http://ww3.sinaimg.cn/large/0060lm7Tgw1f8hqbgormlg30cs0fuh4t.gif)


### License
MIT License
