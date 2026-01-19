# OPEN API

> [!IMPORTANT]
> token 由启动变量 **CMS_API_TOKEN=cloud_media_sync** 指定


## 添加转存下载

**支持115分享、磁力、ed2k、阿里云盘资源转存下载**

### url

**/api/cloud/add_share_down_by_token**

POST请求json传参

### body

```json
{
    "url": "115分享、磁力、ed2k、阿里云盘分享",
    "token": "cloud_media_sync"
}
```

### 响应

```json
{
    "code": 200,
    "msg": "添加转存下载任务成功"
}
```



## 增量同步

**用于触发一次cms的增量同步**

### url

**/api/sync/lift_by_token?type=lift_sync&token=cloud_media_sync**

GET请求

### 响应

```json
{
    "code": 200,
    "msg": "创建任务成功"
}
```


## 增量同步+自动整理

**用于触发一次cms的增量同步+自动整理**

### url

**/api/sync/lift_by_token?type=auto_organize&token=cloud_media_sync**

GET请求

### 响应

```json
{
    "code": 200,
    "msg": "创建任务成功"
}
```