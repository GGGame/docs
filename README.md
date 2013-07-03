docs
====

docs

1. 移植canvas游戏到eject时，需要的移植index.html的资源引用到index.js，采用ejecta.include();
2. 获取ejecta的canvas的方法：document.getElementById('canvas')
3. 多行注释写在对象声明上可能会导致“No or empty script givent” __Error__ 

```javascript
var obj = {
              /**
              * 多行注释
              **/
              "name" : "Object",
              "type" : "Object"
        }
```
