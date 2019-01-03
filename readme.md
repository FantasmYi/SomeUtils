# 这里记录了一些常用的工具类    
##  [HttpClient](https://github.com/FantasmYi/SomeUtils/blob/master/HttpClient.java)
* 可以用这个工具类去跑通一个get或post类型的接口   
* 示例：     
```java  
post类型：   
String url = "http://xxxxxxxxxxxxxxxxxxxxxxxx?id=" + id;
Map<String, String> header = new HashMap<String, String>();
header.put("accept", "text/html, application/json, image/jxr, */*");
String s = HttpClient.sendPost(url, header, null, null, null, null); 
  
get类型：   
String url = "http://XXXXXXXXXXXXXXXXXXXX";
String s = HttpClient.sendGet(url, null);
```
