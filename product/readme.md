# 木犀产品展示API

> 在校园通中展示木犀产品

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/product/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    {
       "_product": [
            {
                "name": "学而",
                "icon": "icon-urlxxxx",
                "url": "https://xueer.muxixyz.com",
                "intro": "华师课程经验挖掘机",
            },
            {....}
        ],
       "update": "时间戳"
    }

## Status Code

    200 OK
    502 服务器端异常

## Notes
