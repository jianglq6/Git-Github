# 写好Git commit message

### 使用Commitizen工具
Commitizen 可以让你的 commit message 更加规范统一，适合项目团队使用，使用也很简单，使用npm安装后，提交代码的时候使用 ```git cz``` 去替代以前的 ```git commit``` 命令即可。

安装commitizen
``` shell
$ sudo npm install -g commitizen
```

### 自动生成Change log
conventional-changelog 是用来从git的元数据中生成 Change log 文档的工具，只要你提交的格式满足它定义的标准，此处以 angular 标准为例子。使用它生成的 Change log 包含以下三个部分：
- Bug Fixes Bug 修复的信息
- Features 增加的特性
- BREAKING CHANGES 重大变更

使用如下：
``` shell
$ sudo npm install -g conventional-changelog-cli
$ cd my-progect
$ conventional-changelog -p regular -i CHANGLOG.md -s
```
这不会覆盖你之前的 CHANGELOG.md 文档内容，会在这个文件的最上面插入新生成的日志信息。
