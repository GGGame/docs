docs
====

docs

1. 移植canvas游戏到ejecta时，需要的移植index.html的资源引用到index.js，采用 __ejecta.include()__ ;
2. 获取ejecta的canvas的方法： __document.getElementById('canvas')__ 
3. 多行注释写在对象声明上可能会导致 __“No or empty script given” Error__ 

```javascript
var obj = {
              /**
              * 多行注释
              **/
              "name" : "Object",
              "type" : "Object"
        }
```
