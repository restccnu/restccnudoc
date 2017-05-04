# 空闲教室API

> 更新空闲教室表

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/classroom/update_classroom/ | 无 | POST |

<hr/>

## URL Params

    无

## POST Data(json)

    无

## Return Data(json)

    {
       "task_id": "xxxxxxxxxxxxx" # 更新任务的id
    }

## Status Code

    201 已创建任务
    502 服务器端异常

---

> 获取空闲教室表更新状态

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/classroom/update_classroom/ | 无 | GET |

<hr/>

## URL Params

    task_id: "xxxxxxxx" # 更新任务的id

## POST Data(json)

    无

## Return Data(json)

    无

## Status Code

    202 已完成更新
    204 更新未完成
    502 服务器端异常

## Notes
