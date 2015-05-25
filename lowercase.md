# 路径和属性要小写

为了和域名命名规则保持一致，使用小写字母并用`-`分割路径名字，例如：

```
service-api.com/users
service-api.com/app-setups
```

属性也使用小写字母，但是属性名要用下划线`_`分割，以便在Javascript中省略引号。 例如：

```json
service_class: "first"
```