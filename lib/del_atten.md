# 取消关注图书API

> 取消关注图书

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
|  /api/lib/del_atten/ | 图书馆登录header | DELETE |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "book_name": 图书名字
    }

## Return Data(json)

    {}

## Status Code

    200 OK
    403 禁止访问
    404 未找到图书
    502 服务器端错误

## Notes
