# 关注图书API

> 关注图书

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
|  /api/lib/attention/ | 图书馆登录header | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "bar_code": 图书编号,
        "book_name": 图书名字,
        "author": 作者名
    }

## Return Data(json)

    {}

## Status Code

    201 OK
    403 禁止访问
    409 已关注

## Notes
