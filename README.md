docs
====

### Notice

1. 移植canvas游戏到ejecta时，需要的移植index.html的资源引用到index.js，采用 __ejecta.include()__ ;
2. 获取ejecta的canvas的方法： __document.getElementById('canvas')__ 
3. 多行注释写在对象声明上可能会导致 __“No or empty script given” Error__ 
4. Ejecta的Audio并不支持 __ogg__ 音频格式
5. Ejecta的Audio.canPlayType 如果不支持的格式返回参数是undefined
6. 在Ejecta使用CAAT.Director初始化的时候，canva传递一个'canvas'字符串
7. 对象直接量的声明内的出现多行注释会导致执行错误

```javascript
var obj = {
              /**
              * 多行注释
              **/
              "name" : "Object",
              "type" : "Object"
        }
```

### CAAT

##### structure

```
CAAT.Foundation.Director + 
	CAAT.Foundation.Scene + 
		CAAT.Foundation.Actor *
    		CAAT.Foundation.ActorContainer *
	    		CAAT.Foundation.ActorContainer *
				CAAT.Foundation.Actor *
```
