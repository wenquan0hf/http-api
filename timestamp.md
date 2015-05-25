# 提供标准的时间戳

为资源提供默认的创建时间 `created_at` 和更新时间 `updated_at`，例如:

```json
{
  ...
  "created_at": "2012-01-01T12:00:00Z",
  "updated_at": "2012-01-01T13:00:00Z",
  ...
}
```

有些资源不需要使用时间戳那么就忽略这两个字段。