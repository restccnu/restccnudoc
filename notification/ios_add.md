# IOS推送API

> 注册IOS设备id

| URL | Header | Method |
| ------ | :------- | :------ |
| /api/push/register/ | 管理员header | POST |

## URL Params

    无

## POST Data(json)

    {
        "unique_id": "ios unique id"
    }

## Return Data(json)

    {
        "message": "add new unique_id"
    }

## Status Code

    201: 创建成功
    403: 禁止访问
    502: 服务器端异常

