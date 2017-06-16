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
