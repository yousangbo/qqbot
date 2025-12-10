# QQ官方机器人PHP框架
## 项目简介
基于PHP开发的QQ官方机器人对接框架，零额外依赖，仅需在QQ官方机器人后台配置回调地址即可快速启用，支持视频、图片、语音、大图、跳转卡片、文卡等多种消息格式，内置公共词库共享功能，整体开发简洁易上手，适合各类QQ机器人开发需求。

## 核心信息
- 开发者：桑帛（忆安）
- 官方交流群：516666275
- 核心API地址：https://api.lolimi.cn
- 公共词库仓库：https://api.lolimi.cn/qqbot/（可自由上传自定义词库，也能下载他人共享词库）
- 框架介绍视频：【QQ官方机器人bot管理系统php框架-写的我好累终于也算是写完了啊哈哈哈哈-哔哩哔哩】https://b23.tv/D5pVysd
- 合规声明：严禁使用本项目开发违规、违法用途的机器人，违者后果自负
- 加密说明：核心代码加密处理，仅为防止二次修改后商用售卖，保障原创权益，感谢理解

## 环境搭建与对接流程
1. 环境要求：必须使用PHP 7.4版本，推荐使用宝塔面板管理，需在宝塔PHP拓展管理中安装sg16拓展；
2. 对接步骤：登录QQ官方机器人后台（https://q.qq.com/），进入「开发设置-回调配置」，订阅方式选「WebHook」，填写框架对应服务回调地址（仅支持80、443、8080、8443端口），勾选所需监听事件（建议全选），提交后等待官方验证通过即可使用。

## 消息格式完整示例
### 基础文本对话
%QQ%
哇塞
你哇塞
干什么

哇
哇什么哇
干什么

### 视频消息（单/多视频）
视频测试
$视频 https://api.lolimi.cn/API/xjj/xjj.php$

多视频测试
$视频 https://api.lolimi.cn/API/xjj/xjj.php$
$视频 https://api.lolimi.cn/API/xjj/xjj.php$

### 图片消息（单/多图片）
图片测试
$图片 https://cravatar.cn/avatar/491ae7135aa925ebece27cf733dd9a68?s=96&d=mp&r=g$

多图片测试
$图片 https://cravatar.cn/avatar/491ae7135aa925ebece27cf733dd9a68?s=96&d=mp&r=g$
$图片 https://cravatar.cn/avatar/491ae7135aa925ebece27cf733dd9a68?s=96&d=mp&r=g$

### 语音消息
语音测试
$语音 https://apii.lolimi.cn/api/tryyhc/data/6e38f66863.mp3$

### 大图消息
大图
$大图 风景 描述 https://img.lolimi.cn/thumbnails/936a75c7f89b7e0b217cacf1b8cb8876.png$

### 跳转卡片消息
跳转卡片
$跳转卡 百度 搜索 https://img.lolimi.cn/thumbnails/936a75c7f9b7e0b217cacf1b8cb8876.png 0$

### 文卡消息
文卡
$文卡 风景|1 风景|1 测试文本$
