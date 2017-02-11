# 图书可借API

> 图书可借

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
|  /api/lib/get_atten/ | 图书馆登录header | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    {
        'book_list': ["平凡的世界", "计算机网络"]
    }

## Status Code

    200 OK
    403 禁止访问
    404 无关注图书或关注图书均不可借
    502 服务器端错误

## Notes
