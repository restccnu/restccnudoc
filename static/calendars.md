# 校历API

> 获取校历

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/calendar/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    [
        {
          "img": "http://muxistatic.com",    // 图片七牛外链
          "size": "高x宽", # x 是一个 爱克斯
          'update': 时间戳                   // 图片更新时间戳
        },
        {....}
    ]

## Status Code

    200 OK
    502 服务器端异常

## Notes
