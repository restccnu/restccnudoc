# 添加课表API

> 添加课程

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/table/ | 信息门户登录header | GET |

<hr/>

## Headers
信息门户登录headers(注意大小写)

    'Bigipserverpool_Jwc_Xk':'139503808.20480.0000'
    'Sid':'2014210761'
    'Jsessionid': 'B6A6DF5C48AB4AD4C4001572D2611809'

## URL Params

    无

## POST Data(json)

    {
        "course": "xxxx",  // 课程的名称
        "teacher": "xxxx",  // 老师的名称
        "weeks": "1, 2, 3,,,,,19",  // 上课周次
        "day": "1",  // 上课星期(1~7)
        "start": "3", // 课程开始时间(ex: start=3表示上午第三节课开始上)
        "during": "2", // 课程持续时间(ex: during=2表示持续2节课)
        "place": "9-21", // 上课地点
        "remind": false // 是否提醒
    }

## Return Data(json)

    {"id": id} // 自定义课程存储ID

## Status Code

    201: 创建成功
    403: 禁止访问
    502: 服务器端异常
    401: 未授权

## Notes
