
# 单元测试：检测最小可测试单元

单元测试，是指对系统中的最小可测试单元进行检查和验证。

每个类、组件、服务等开发，可以在xxx.component.spec.ts文件中，编写单元测试用例

单元测试示例：
- src\app\app.component.spec.ts
- src\modules\bvideo\home\home.component.spec.ts

编写规则详解：
- 编译阶段：通过组件是否正常编译，判断是否成功
- 属性加载：通过判断组件内属性及方法的预测值，判断是否成功
- 页面渲染：通过页面中可能存在的HTML元素及内部值，判断是否成功

# FAQ:CHROME_BIN环境变量未设置
解决方案：
```
#!/bin/sh
export CHROME_BIN="chromium"
```

问题描述：
``` sh
To disable this warning use "ng config -g cli.warnings.versionMismatch false".
✔ Browser application bundle generation complete.
11 12 2022 14:25:02.107:WARN [karma]: No captured browser, open http://localhost:9876/
11 12 2022 14:25:02.123:INFO [karma-server]: Karma v6.4.1 server started at http://localhost:9876/
11 12 2022 14:25:02.123:INFO [launcher]: Launching browsers Chrome with concurrency unlimited
11 12 2022 14:25:02.126:INFO [launcher]: Starting browser Chrome
11 12 2022 14:25:02.128:ERROR [launcher]: No binary for Chrome browser on your platform.
  Please, set "CHROME_BIN" env variable.
```