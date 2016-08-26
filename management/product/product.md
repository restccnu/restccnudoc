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
       "upate": "时间戳"
    }

## Status Code

    200 OK
    502 服务器端异常

## Notes

<hr/>

# 木犀产品删除API

> 删除一个校园通上展示的木犀产品

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/product/?name=学而 | 管理员登录header | DELETE |

<hr/>

## URL Params

    name: 待删除产品的名称

## POST Data(json)

    无

## Return Data(json)

    {}, 200

## Status Code

    200 OK
    404 name对应的产品不存在
    403 禁止访问

## Notes

<hr/>

# 木犀产品添加API

> 添加一个木犀产品展示

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/product/ | 管理员登录header | PUT |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "name": "产品名称",
        "icon": "学而icon七牛外链",
        "url": "产品url",
        "intro": "产品介绍"
    }

## Return Data(json)

    {}, 200

## Status Code

    200 OK
    403 禁止访问

## Notes
