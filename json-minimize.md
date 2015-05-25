# 保证响应 JSON 最小化

请求中多余的空格会增加响应大小，而且现在很多的 HTTP 客户端都会自己输出可读格式（"prettify"）的JSON。所以最好保证响应 JSON 最小化，例如：

```json
{"beta":false,"email":"alice@heroku.com","id":"01234567-89ab-cdef-0123-456789abcdef","last_login":"2012-01-01T12:00:00Z","created_at":"2012-01-01T12:00:00Z","updated_at":"2012-01-01T12:00:00Z"}
```

而不是这样：

```json
{
  "beta": false,
  "email": "alice@heroku.com",
  "id": "01234567-89ab-cdef-0123-456789abcdef",
  "last_login": "2012-01-01T12:00:00Z",
  "created_at": "2012-01-01T12:00:00Z",
  "updated_at": "2012-01-01T12:00:00Z"
}
```

你可以提供可选的方式为客户端提供更详细可读的响应，使用查询参数（例如：`?pretty=true`）或者通过`Accept`头信息参数（例如：`Accept: application/vnd.heroku+json; version=3; indent=4;`）。
