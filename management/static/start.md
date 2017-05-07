# 闪屏API

> 闪屏

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/start/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    {
        "img": "http:xxxxxxxxx",  // 闪屏图片外链
        "url": "xxxxxxxxxxxxxx",  // 图片指向链接
        "update": timestamp       // 图片更新时间戳
    }

## Status Code

    200 OK
    502 服务器端异常

## Notes

<hr/>

# 更新闪屏API

> 更新闪屏

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/start/ | 管理员登录header | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "img": "闪屏图片外链",
        "url": "闪屏指向的链接"
    }

## Return Data(json)

    {}, 201

## Status Code

    201: 创建成功
    403: 禁止访问
    502: 服务器端异常

## Notes
