# 图书搜索API

> 图书搜索

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/lib/search/?keyword=xxx&page=1 | 无| GET |

<hr/>

## URL Params

    keyword: 搜索词(作者、书名...)
    page: 查询页. 搜索结果会进行分页, 每页20条记录, 默认page为第一页

## POST Data(json)

    无

## Return Data(json)

    {
      "meta": {
           "max": 2  // 最大页数
           "per_page": 20  // 平均每页
       }
       "results": [
           {
               "book": "xxxx",  // 书名
               "author": "xxxx", // 作者名
               "bid":  "xxxxxxxxxxx", // 图书索书号
               "intro": "xxxxxxx", // 图书介绍(部分图书没有介绍)
               "id": "xxx"  // 图书的id(标识每一本图书)
           },
           {....},
       ]
    }

## Status Code

    200 OK
    502 服务器端异常

## Notes
