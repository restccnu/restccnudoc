# 课表查询API

> 获取课表

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/table/ | 信息门户登录cookie | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "cookie": {
            "BIGipServerpool_jwc_xk": "407939264.20480.0000", 
            "JSESSIONID": "26A06E720057BEABF52AF32F616B9644"
        },
        "sid": "2014210761",
    }

## Return Data(json)

    [
     {
        "id": "1", // 课程id
        "course": "xxxx", // 课程名称
        "teacher": "xxxx", // 老师名
        "weeks": "1, 2, 3,,,,,19", // 上课周
        "day": 1, // 上课日: 星期1~7
        "start": 1, // 每天课程开始时间(ex: start=1 表示早上第一节课开始)
        "during": "2",  // 课程持续时间(ex: during=2 表示课程持续2节课)
        "place": "9-21",  // 上课地点
        "remind": true/false # 课程是否设置为提醒。用户自定义课程可以设置提醒, 信息门户课程设为false。
        "color": 0或1或2或3, # 课程格子的颜色(随机生成)
     },
     {...} ,
    ]

## Status Code

    200 Ok
    403 禁止访问
    502 服务器端异常

## Notes
