# 管理IOS json配置API

> 管理ios json配置; 上传、更新

# 上传ios json配置

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ios/config/ | 管理员header |  POST |

<hr/>

## URL Params

    无

## POST Data(json)

    {"config": "{'k1':'v1', 'k2':'v2'}"}    # ios json配置
    
## Return Data(json)

    {}
    
## Status Code

    成功上传: 201

# 更新ios json配置

| URL |  Header | Method |
| ------------- |:-------------:| -----:|
| /api/ios/config/ | 管理员header |  PUT |

<hr/>

## URL Params

    无

## POST Data(json)

    {"config": "{'k1':'v1', 'k2':'v2', 'k3':'v3'}"}    # ios json配置
    
## Return Data(json)

    {}
    
## Status Code

    成功更新: 200
    配置不存在: 404

## Notes
