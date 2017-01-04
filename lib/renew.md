# 图书续借API

> 图书详情

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/lib/?bar_code=xxxx&check=xxxx | 无 | GET |

<hr/>

## URL Params

    bar_code: 图书编号
    check: 图书check号码

## POST Data(json)

    无

## Return Data(json)

    {}

## Status Code

    200 续借成功
    404 不到续借时间
    403 超过最大续借次数
    400 请求无效

## Notes
