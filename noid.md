# 支持方便的无 id 间接引用

在某些情况下，让用户提供 ID 去定位资源是不方便的。例如，一个用户想取得他在 Heroku 平台 app 信息，但是这个 app 的唯一标识是 UUID。这种情况下，你应该支持接口通过名字和 ID 都能访问，例如:

```
$ curl https://service.com/apps/{app_id_or_name}
$ curl https://service.com/apps/97addcf0-c182
$ curl https://service.com/apps/www-prod
```

不要只接受使用名字而放弃了使用 id。