后台controller层接口入参不同复杂程度的参数传递指南

## Get请求

@RequestParam 用以匹配 method/paramKey=paramVal 结构的请求路径

@PathVariable 用以匹配 method/paramVal1/paramVal2 结构的请求路径

以上两个参数皆有

### 单个参数

**前端入参：**

```
http://localhost:8080/singleParam?str=good
```

**接口入参：**

这里的`@RequestParam`如果不加，则默认匹配`str`

```java
@GetMapping("singleParam")
public Rs singleParam(@RequestParam("str") String str) {
  if (StringUtils.hasText(str)) {
    return Rs.success("传参成功");
  }

  return Rs.fail("传参失败");
}
```





### RESTFul风格单个参数

**前端入参：**

```
http://localhost:8080/singleParam1/good
```

**接口入参：**

```java
@GetMapping("singleParam1/{str}")
public Rs singleParam1(@PathVariable String str) {
  if (StringUtils.hasText(str)) {
    return Rs.success("传参成功");
  }

  return Rs.fail("传参失败");
}
```



### 单个对象

前端入参：

```
http://localhost:8080/passObject?age=1&name=1
```

接口入参：

```java
@GetMapping("passObject")
public Rs passObject(User user) {
  if (user != null && StringUtils.hasText(user.getName())) {
    return Rs.success("传参成功");
  }

  return Rs.fail("传参失败");
}
```



### 单个基础数据类型数组

**前端参数：**

```
http://127.0.0.1:8081/singleParamArray?str=1,2,3
http://127.0.0.1:8081/singleParamArray?str=1&str=2&str=3
```

**接口入参：**

```java
@GetMapping("singleParamArray")
public Rs singleParamArray(String[] str) {
  if (str != null && str.length > 0) {
    return Rs.success("传参成功");
  }

  return Rs.fail("传参失败");
}
```

### 单个对象数组

使用get请求无法传递对象数组



### 多个基础参数

与传单个参数类似，故不写



### 多个RESTFul风格的基础参数

与传单个类似，故不写



### 多个基础数据类型数组

... 故不写



### 多个对象

















