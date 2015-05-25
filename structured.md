# 生成结构化的错误

响应错误的时，生成统一的、结构化的错误信息。包含一个机器可读的错误 `id`，一个人类能识别的错误信息（`message`），根据情况可以添加一个`url`来告诉客户端关于这个错误的更多信息以及如何去解决它，例如:

```
HTTP/1.1 429 Too Many Requests
```

```json
{
  "id":      "rate_limit",
  "message": "Account reached its API rate limit.",
  "url":     "https://docs.service.com/rate-limits"
}
```

文档化客户端可能遇到的错误信息格式，以及这些可能的错误信息`id`。