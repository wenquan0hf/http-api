# 可读性

## 机器可读的 JSON 模式

提供一个机器可读的模式可以精确的指定你的 API。使用 prmd 来管理你的模式，并确保它能被prmd verify 验证。

## 人类可读的文档

提供人类可读的文档让客户端开发人员可以理解你的 API。

如果你用 prmd 创建了一个概要并且按上述要求描述，你可以为所有节点很容易的使用`prmd doc`生成 Markdown文档。

除了节点信息，提供一个 API 概述信息:

- 验证授权，包含如何取得和如何使用 token。
- API 稳定及版本管理，包含如何选择所需要的版本。
- 一般情况下的请求和响应的头信息。
- 错误的序列化格式。
- 不同编程语言客户端使用 API 的例子。