# 获取补丁包版本API

> 返回所有补丁包版本(包括历史版本)的相关信息

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/patch/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    [
        {
           "version": "v1",  //  版本号,
           "download": "http://xxx.com",  // 下载地址
           "update": "2016-0802",  // 更新时间
           "intro": "这是一次史无前例的更新", // 更新说明
           "size": "100M"  // 补丁包大小
        },
        {...},
    ]

## Status Code

    200 OK
    502 服务器端异常

## Notes

<hr/>

# 获取最新的补丁包版本API

> 获取最新的补丁包版本信息

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
|  /api/patch/latest/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    {
      "version": "v1",  # 版本号,
      "download": "http://xxx.com",  # 下载地址
      "update": "2016-0802",  # 更新时间
      "intro": "这是一次史无前例的更新", # 更新说明
      "size": "100M"  # 补丁包大小
    }

## Status Code

    200 OK
    502 服务器端异常

## Notes

<hr/>

# 添加补丁包版本API

> 添加一个新的补丁包P版本

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/patch/ | 管理员登录header | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
       "version": "v1",  # 版本号,
       "download": "http://xxx.com",  # 下载地址
       "update": "2016-0802",  # 更新时间
       "intro": "这是一次史无前例的更新", # 更新说明
       "size": "100M"  # 补丁包大小
    }

## Return Data(json)

    {'msg': 'add new patch version data'}, 201

## Status Code

    201 添加成功
    403 禁止访问
    502 服务器端异常

## Notes

<hr/>

# 删除补丁包版本API

> 删除特定版本的补丁包信息

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/patch/<str:version>/ | 管理员登录header | DELETE |

<hr/>

## URL Params

    version: 版本号

## POST Data(json)

    无

## Return Data(json)

    {'msg': 'delete patch version 版本号'}, 200

## Status Code

    200 OK
    403 禁止访问
    502 服务器端异常

## Notes
