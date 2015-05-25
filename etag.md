# 支持 Etag 缓存


```
, identifying the specific

version of the returned resource. The user should be able to check for

staleness in their subsequent requests by supplying the value in the

If-None-Match header.
```

在所有的请求中带上 ETag 头 ， 用于识别特定版本的返回资源。用户可以在随后的请求中通过提供 `If-None-Match `头的值来检查内容是否过期。