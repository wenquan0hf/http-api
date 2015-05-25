# 提供可执行的例子

提供可执行的示例让用户可以直接在终端里面看到 API 的调用情况，最大程度的让这些示例可以简单的使用，以减少用户尝试使用 API 的工作量。例如:

```
$ export TOKEN=... # acquire from dashboard
$ curl -is https://$TOKEN@service.com/users
```

如果你使用[prmd](https://github.com/interagent/prmd)生成 Markdown 文档，每个节点都会自动获取一些示例。