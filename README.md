# 管理台vue模版


### 介绍

1.  fork直接可用
2.  基于vue-cli3构建
3.  利用 eslint 规范代码
4.  利用 husky 规范 git 提交记录


### 项目开发


1.  依赖安装
```
tnpm install
```

2.  项目启动
```
npm run serve
```

3.  打包编译（本地不需要做，sumeru编译容器里做）
```
npm run build
```

4.  eslint修复问题
```
npm run lint
```

### 登录

1.  统一走公司智能网管
2.  将下载下来的 xxxxx.txt 文件放到根目录

### 上线部署

1.  修改pre-deploy.sh
2.  移动从智能网管下载的 xxxxx.txt 文件到dist目录



## 流程规范：

### 一、采用eslint，开启代码规范检查

1.  代码锁进： 4个空格。
2.  导出，引入模块请使用 export和import.
3.  语句结束，分号可以加，也可以不加。
4.  未使用的变量禁止定义。
5.  未使用的模块，禁止导入。
6.  字符串必需使用单引号。
7.  模版字符串请使用反引号(``)。
8.  路径拼接请使用 path.join



### 二、增加 git 钩子函数
1.  代码commit前，会首先进行代码格式检测，如果检测不通过，无法提交代码。

2.  目前只在commit加了钩子。

3.  禁止在主分支commit代码

#   请大家遵守以上规范，不要修改eslintrc文件。谢谢。


