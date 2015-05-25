# 显示频率限制状态

客户端的访问速度限制可以维护服务器的良好状态，保证为其他客户端请求提供高性的服务。你可以使用[token bucket algorithm](http://en.wikipedia.org/wiki/Token_bucket)技术量化请求限制。

为每一个带有`RateLimit-Remaining`响应头的请求，返回预留的请求 tokens。