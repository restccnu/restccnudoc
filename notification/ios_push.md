# IOS推送API

> 推送API

| URL | Header | Method |
| ------ | :------- | :------ |
| /api/push/ | 管理员header | POST |

## URL Params

    无

## POST Data(json)

    {
        "title": "xxxx"
    }

## Return Data(json)

    无:

    如果出错返回错误的设备token和相应信息
    {
        error_token: error_message
    }

## Status Code

    201: 创建成功
    403: 禁止访问
    502: 服务器端异常

