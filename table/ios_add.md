# 添加课表API (IOS版临时)

> 添加课程

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ios/table/ | 信息门户登录header | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {
        "course": "xxxx",  // 课程的名称
        "teacher": "xxxx",  // 老师的名称
        "weeks": "1, 2, 3,,,,,19",  // 上课周次
        "day": "星期1",  // 上课星期(1~7)
        "start": "3", // 课程开始时间(ex: start=3表示上午第三节课开始上)
        "during": "2", // 课程持续时间(ex: during=2表示持续2节课)
        "place": "9-21", // 上课地点
        "remind": false // 是否提醒
    }

## Return Data(json)

    无

## Status Code

    201: 创建成功
    403: 禁止访问
    502: 服务器端异常

## Notes

    由于mongodb的特性: 数据存在才会创建数据库, 所以内含id为0的占位课程(re:0)

