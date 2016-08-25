# 获取app版本API

> 返回所有版本(包括历史版本)的相关信息

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/app/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    [
        {
            "name": "华师匣子",
            "version": "v1",  // 版本号,
            "download": "http://xxx.com",  // 下载地址
            "update": "2016-0802",  // 更新时间
            "intro": "这是一次史无前例的更新", // 更新说明
            "size": "100M"  // 更新包大小
        },
        {...},
    ]

## Status Code

    200 OK
    502 服务器端异常

## Notes

<hr/>

# 获取最新的APP版本API

> 获取最新的APP版本信息

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
|  /api/app/latest/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    {
       "name": "华师匣子",
       "version": "v1",  // 版本号,
       "download": "http://xxx.com",  // 下载地址
       "update": "2016-0802",  // 更新时间
       "intro": "这是一次史无前例的更新", // 更新说明
       "size": "100M"  // 更新包大小
    }

## Status Code

    200 OK
    502 服务器端异常

## Notes

<hr/>

# 添加版本API

> 添加一个新的APP版本

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/app/ | 管理员登录header | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
      "name": "华师匣子",
      "version": "v1",  # 版本号,
      "download": "http://xxx.com",  # 下载地址
      "update": "2016-0802",  # 更新时间
      "intro": "这是一次史无前例的更新", # 更新说明
      "size": "100M"  # 更新包大小
    }

## Return Data(json)

    {'msg': 'add new version data'}, 201

## Status Code

    201 添加成功
    403 禁止访问
    502 服务器端异常

## Notes

<hr/>

# 删除app版本API

> 删除特定版本的app信息

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/app/<str:version>/ | 管理员登录header | DELETE |

<hr/>

## URL Params

    version: 版本号

## POST Data(json)

    无

## Return Data(json)

    {'msg': 'delete version 版本号'}, 200

## Status Code

    200 OK
    403 禁止访问
    502 服务器端异常

## Notes
