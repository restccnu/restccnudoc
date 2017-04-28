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
        [ // 所有关注的图书
            {
            "bid": "xxxx", // 图书的bid
            "book": "xxxx", // 图书的名字
            "id": , "xxxx", // 图书的id
            "author": "xxxx", // 图书的作者
            "avbl": "y" // 图书是否可借("y"/"n")
            },
            { ... }
        ]
    }

## Status Code

    200 OK
    403 禁止访问
    404 无关注图书
    502 服务器端错误

## Notes
