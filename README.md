# HTTP API 设计指南

这篇指南介绍描述了 HTTP+JSON API 的一种设计模式，最初摘录整理自 Heroku 平台的 API 设计指引 [Heroku 平台 API 指引](https://devcenter.heroku.com/articles/platform-api-reference)。

这篇指南除了详细介绍现有的 API 外，Heroku 将来新加入的内部 API 也会符合这种设计模式，我们希望非 Heroku 员工的 API 设计者也能感兴趣。

我们的目标是保持一致性，专注业务逻辑同时避免过度设计。我们一直试图找出一种良好的、一致的、显而易见的 API 设计方法，而并不是所谓的"最终/理想模式"。

## 学习前提

我们假设你熟悉基本的 HTTP+JSON API 设计方法，所以本篇指南并不包含所有的 API 设计基础。

鸣谢：[https://github.com/ZhangBohan/http-api-design-ZH_CN/blob/master/README.md](https://github.com/ZhangBohan/http-api-design-ZH_CN/blob/master/README.md)
