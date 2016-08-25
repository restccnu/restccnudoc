# 我的图书馆API

> 我的图书馆

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
|  /api/lib/me/ | 图书馆登录header | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    [
        // 我借阅的所有书籍
        {
            "book": 'xxx', // 图书名称
            "author": 'xxx',  // 作者名称
            "itime": 'y-m-d', // 借阅日期
            "otime": 'y-m-d', // 归还日期
            "time": '10'  // 距离归还日剩余天数(过期显示为负数)
        },
        {.....},
    ]

## Status Code

    200 OK
    403 禁止访问
    502 服务器端异常

## Notes

    现在学校图书馆网站处于崩溃状态...
