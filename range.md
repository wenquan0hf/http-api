# 通过请求中的范围（Range）拆分大的响应

一个大的响应应该通过多个请求使用`Range`头信息来拆分，并指定如何取得。详细的请求和响应的头信息（header），状态码(status code)，范围(limit)，排序(ordering)和迭代(iteration)等，参考[Heroku Platform API discussion of Ranges](https://devcenter.heroku.com/articles/platform-api-reference#ranges)。
