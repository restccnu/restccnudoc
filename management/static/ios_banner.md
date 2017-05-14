# Banner获取API

> 获取banner

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ios/banner/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    [
        {
          "img": "http://muxistatic.com",  // 图片外链
          "url": "http://muxistudio.com",  // 图片指向链接
          "num": "1",                      // Banner排序的数字戳(越小越先出现)
          'update': 时间戳                 // 图片更新时间戳
        },
        {....}
    ]

## Status Code

    200 OK
    502 服务器端异常

## Notes

<br/>

# 添加banner API

> 添加banner

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ios/banner/ | 管理员登录header | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        'img': 'banner图片外链',
        'url': 'banner指向的链接',
        "num": 排序(越小越先出现, 最小为1)
    }

## Return Data(json)

    {}, 201

## Status Code

    201 创建成功
    403 禁止访问
    502 服务器端异常

## Notes

<br/>

# 删除banner API

> 根据文件名删除banner

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ios/banner/ | 管理员登录header | DELETE |

<hr/>

## URL Params

    name: 待删除的banner图片外链

## POST Data(json)

    无

## Return Data(json)

    {}, 200

## Status Code

    200 OK
    404 该文件找不到
    403 禁止访问
    502 服务器端异常

## Notes

# 更新banner API

> 更新banner排序

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ios/banner/ | 管理员header | PUT |

<hr/>

## URL Params

    无

## PUT Data(json)

    {
        "img": "http://muxistatic.com",    // 待修改banner外链
        "num": 1                           // 更新后的排序num
    }

## Return Data(json)

    {}, 200

## Status Code

    200 OK
    404 待修改的banner不存在
    502 服务器端异常

## Notes
