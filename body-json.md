# 在请求的 body 体使用 JSON 格式数据

在 `PUT`/`PATCH`/`POST` 请求的正文（request bodies）中使用JSON格式数据，而不是使用 form 表单形式的数据。这与我们使用JSON格式返回请求相对应，例如:

```
$ curl -X POST https://service.com/apps \
    -H "Content-Type: application/json" \
    -d '{"name": "demoapp"}'

{
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "name": "demoapp",
  "owner": {
    "email": "username@example.com",
    "id": "01234567-89ab-cdef-0123-456789abcdef"
  },
  ...
}
```