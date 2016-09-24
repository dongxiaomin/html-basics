# 面试题
## js
```javascript
	var fn = function(){
	  a = 1;
	  d = 2;
	}
	console.log(d);
	
	打印出：Uncaught ReferenceError: d is not defined(…)    /*报错*/
```

```javascript	
	var name = 'zhangsan';
	var fn = (function(name){
	  return function(){
	    if( typeof name == 'undefined' ){
	      var name = 'lisi';
	      console.log('hello ' + name);
	    }else{
	      console.log('hello ' + name);
	    }
	  }
	})(name);
	fn();

	打印出：hello lisi
```