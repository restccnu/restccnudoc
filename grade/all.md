# 总成绩查询API

> 总成绩查询

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/grade/search/?xnm=2015&xqm=3 | 信息门户登录header | GET |

<hr/>

## URL Params

    xnm: xnm年-xxx年, 例如2015-2016学年那么xnm=2015
    xqm: 第一学期 xqm=3, 第二学期 xqm=12, 第三学期 xqm=16

## POST Data(json)

    无

## Return Data(json)

    [
       {
           "course": "xxx",  // 课程
           "credit": "xxx",  // 学分
           "grade" : "80",   // 总评
           "category": "专业必修课", // 课程类别
           "type": "文", // 课程分类
           "jxb_id": "1", # 一个奇怪的id, 用于该课程成绩详情API查询
           "kcxzmc": "专业必修课" # 课程属性
       },
       {....}
    ]

## Status Code

    200 ok
    403 禁止访问
    502 服务器端异常

## Notes
