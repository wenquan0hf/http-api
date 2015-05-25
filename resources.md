# 提供全部可用的资源

提供全部可显现的资源 (例如： 这个对象的所有属性) ，当响应码为 200 或是 201 时返回所有可用资源，包含 `PUT`/`PATCH` 和 `DELETE`
请求，例如:


```json
$ curl -X DELETE \
  https://service.com/apps/1f9b/domains/0fd4

HTTP/1.1 200 OK
Content-Type: application/json;charset=utf-8
...
{
  "created_at": "2012-01-01T12:00:00Z",
  "hostname": "subdomain.example.com",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "updated_at": "2012-01-01T12:00:00Z"
}
```

当请求状态码为 202 时，不返回所有可用资源，例如：

```
$ curl -X DELETE \
  https://service.com/apps/1f9b/dynos/05bd

HTTP/1.1 202 Accepted
Content-Type: application/json;charset=utf-8
...
{}
```
