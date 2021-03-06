# tac-cli

这是腾讯云 [MobileLine （移动研发平台）](https://cloud.tencent.com/product/tac) 命令行工具，提供便捷的本地工具，方便做静态网站部署等操作。

## 安装命令行工具

```shell
npm i -g tac-cli
```

## 初始化配置

```shell
tac config
```

这个命令会要求设置 secretId 和 secretKey，可到 [腾讯云控制台](https://console.cloud.tencent.com/cam/capi) 获取

## 列出所有项目

```shell
tac ls
```

## 切换项目

```shell
tac use <projectId>
```

该命令可以指定当前命令生效的项目。

## 上传文件

```shell
tac config
tac use <projectId>
tac deploy ./www
```

如果不传入目录，默认部署当前目录文件

```shell
tac deploy
```

![deploy](https://tacimg-1253960454.cos.ap-guangzhou.myqcloud.com/guides/hosting/命令行工具-静态网站部署.png)
