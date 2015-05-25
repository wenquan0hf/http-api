# 为内省而提供 Request-Id

为每一个请求响应包含一个`Request-Id`字段，并使用 UUID 作为该值。通过在客户端、服务器或任何支持服务上记录该值，它能主我们提供一种机制来跟踪、诊断和调试请求。