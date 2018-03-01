# 信息 

## 添加信息 

|URL| headers|methods|
|--|--|--|
| /api/msg/ | 管理员header  | POST | 

**URL Params:  None** 

**POST Data:** 
```
{
	 "msg" : string   //  简略信息
	 "detail" : string  // 详细信息 
	 "version" : string    // 版本信息
	 "type" : string    // 信息类型 
	 "time" : string  // 2018-02-24   更新时间 
}
``` 

**RETURN Data: None** 

**Status Code** 

```
200      // 成功
500      // 服务器端错误 
401      // 没有管理员header
403      // 禁止访问 
```
 
 ***


## 获取最新信息   

|URL| headers|methods|
|--|--|--|
| /api/msg/ | None | GET | 

**URL Params: None** 
**POST Data: None** 
**RETURN Data:** 
```
{
     "msg" : string   //  简略信息
	 "detail" : string  // 详细信息 
	 "version" : string    // 版本信息
	 "type" : string    // 信息类型 
	 "time" : string  // 2018-02-24   更新时间 
	 "update" : int    // 更新的时间戳 
}
```

或                      // 没有信息 
```
{
     "msg" : ""
	 "detail" : ""
	 "version" : "" 
	 "type" : ""
	 "time" : "" 
	 "update" : 0 
}
```





**Status Code** 
```
200 // 成功 
500 // 服务器端错误 
```

***

## 删除信息 

|URL| headers|methods|
|--|--|--|
| /api/msg/ | 管理员header | DELETE |  

**URL Params:** 
```
    "msg" : string        // 简略信息 
```

**POST Data: None** 

**RETURN Data: None** 

**Status Code:**   

```
200        //  成功 
404        // 信息不存在
500        // 服务器端错误 
401      // 没有管理员header
403      // 禁止访问 
```


