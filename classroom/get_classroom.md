# 空闲教室API

> 获取空闲教室表

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/classroom/get_classroom/?weekno=10&weekday=mon&building=7 | 无 | GET |

<hr/>

## URL Params

    weekno: 周数('1' ~ '20')
    weekday: 星期('mon', 'tue', 'wed', 'thu', 'fri')
    building: 楼栋('7', '8')

## POST Data(json)

    无

## Return Data(json)

    {
      '1': ['7101', '7102']
      '2': ['7101', '7102']
      '3': ['7101', '7102', '7103']
      ...
      '13': ['7104']
      '14': ['7104']
    }

## Status Code

    200 Ok
    502 服务器端异常

## Notes
