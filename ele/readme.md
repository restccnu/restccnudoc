# 电费查询API

> 电费查询

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ele/ | 无 |  POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "dor": "东1-101",
        // dor:
        // 国交K栋0101为: 国K-0101
        // 其他的都是栋前缀+'-'+房号
        // 比如东附1栋101为: 东附1-101
        "type": "air/light"
    }

## Return Data(json)

    {
       "dor": "东1-101",
       "degree": {
            "remain": "xxx", // 剩余度数
            "before": "xxx",   // 上月用电
            "current": "xxx"   // 当月用电
       },
       "ele": {
            "remain": "xxx",   // 剩余电费
            "before": "xxx",   // 上月电费
            "current": "xxx"   // 当月电费
       }
    }

## Status Code

    寝室不存在 返回状态码为: 404
    学校系统崩裂 返回状态码为: 502

## Notes

    学校的电费查询有毒, 使用需谨慎...
