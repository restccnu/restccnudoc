# 图书续借API

> 图书详情

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/lib/renew/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    bar_code: 图书编号
    check: 图书check号码

## Return Data(json)

    {}

## Status Code

    200 续借成功
    406 不到续借时间
    403 超过最大续借次数
    400 请求无效

## Notes
