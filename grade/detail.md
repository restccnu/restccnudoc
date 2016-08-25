# 平时成绩查询API

> 平时成绩查询

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/grade/detail/search/?xnm=2015&xqm=3&course=hacks web开发&jxb_id=1 | 信息门户登录header | GET |

<hr/>

## URL Params

    xnm: xnm年-xxx年, 例如2015-2016学年那么xnm=2015
    xqm: 第一学期 xqm=3, 第二学期 xqm=12, 第三学期 xqm=16
    course: 课程名称
    jxb_id: 一个奇怪的id.. 总成绩查询API会返回

## POST Data(json)

    无

## Return Data(json)

    {
        "usual": "60", # 平时分
        "ending": "60",  # 期末分
    }


## Status Code

    200 OK
    403 禁止访问
    502 服务器端异常

## Notes
