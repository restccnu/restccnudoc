# 关注图书API

> 关注图书

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
|  /api/lib/create_atten/ | 图书馆登录header | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "book_name": 图书名字,
    }

## Return Data(json)

    {}

## Status Code

    201 添加关注成功
    403 禁止访问
    409 已关注
    502 服务器端错误

## Notes
