# 使用以下方法安装

```

npm install -g webpack@~4.15.0 webpack-cli@~3.3.2 webpack-dev-server@~3.4.1 https://github.com/angryreid/vuma.git
```

# API

```
vuma     	# 显示可用API
vuma init 	# 初始化项目目录（默认为fe)
vuma start	# 执行菜单列表
vuma upgrade # 更新vuma工具

```

# 注意事项  && 常见问题

1. 执行vuma-start，启动开发服务器时，出现错误 "Cannot find module 'webpack'"

2. 继续执行vuma-start，选择安装依赖包。

# 开发者注意事项

1. 每次更新需为一项完整功能，并在commit log中注明

2. 版本号规则是x.x.x，遵循GNU版本规则[http://blog.chinaunix.net/uid-22556372-id-1773412.html]

3. 更新版本提交后，必须<font color='#0099ff'>手动修改package.json中的版本号</font>，同时<font color='#0099ff'>生成一个tag名为当前版本号</font>。
	例如版本号为1.0.2,tag为1.0.2。vuma将使用package.json与远程vuma库进行版本对比，非最新版本将再有网状态下自动升级。

```
	操作方式分两步：
		1. 修改vuma库下的package.json => version为最新版本号 x.x.x，并推送
		2. git tag -a x.x.x -m '此处填写该版本的详细变化';git push --tags
```
