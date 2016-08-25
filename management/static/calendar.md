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

    {
        "img": "http://muxistatic.com",    // 图片七牛外链
        "size": "高x宽", # x 是一个 爱克斯
        'update': 时间戳                   // 图片更新时间戳
    },

## Status Code

    200 OK
    502 服务器端异常

## Notes


<hr/>

# 更新校历API

> 更新校历

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/calendar/ | 管理员登录header | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "img": "校历上传到七牛后的文件名",
        "size": "长x宽"  // 校历图片大小, 注意x是埃克斯
    }

## Return Data(json)

    {}, 201

## Status Code

    201: 创建成功
    502: 服务器端异常

## Notes
更新校历会用新的校历替换原有的校历
