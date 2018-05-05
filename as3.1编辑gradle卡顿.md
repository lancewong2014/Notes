#Android Studio 3.1编辑build.gradle文件卡顿问题

[blog link](https://blog.csdn.net/wangluotianxi/article/details/79757558)
原因：Android Studio 一直请求http://search.maven.org/solrsearch/select?等两个接口，造成卡顿。

通过在hosts文件设置映射处理

```
127.0.0.1 search.maven.org
```