# 信息门户登录API

> 对应应用首页的登录

| URL | Header |  Method |
| ------------- |:-------------:| -----:|
| /api/info/login/ | 信息门户登录header | GET |

<hr/>

### URL Params

    无

### POST Data(json)

    无

### Return Data(json)

    {
        "JSSESIONID": "A04ED5EEA6C34A523611376AF52A04A9",
        "BIGipServerpool_jwc_xk": "1028696256.20480.0000",
        "sid": "2014210761"
    }


### Status Code:

    200 OK
    403 禁止访问, 用户验证出错
    502 服务器端错误

### Notes
