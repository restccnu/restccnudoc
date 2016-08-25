# 部门信息API

> 部门信息

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/apartment/ | 无 | GET |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    [
        {
          "apartment": "学生事务大厅",  // 部门名称
          "phone": ["67867510",],   // 部门电话
          "place": "文华公书林东侧二楼" // 部门地点
        }，
        {....}
    ]

## Status Code

    200 OK
    502 服务器端异常

## Notes
部门信息是写死的.. 也是我最有信心的API
