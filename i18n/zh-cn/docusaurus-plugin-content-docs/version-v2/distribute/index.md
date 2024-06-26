---
title: 发布应用
sidebar_position: 1
sidebar_label: 发布应用
---

## 操作流程

![app_process](/img/docs/distribute/app_process.png)

## 应用登记

- 在应用列表页面，选择**创建应用**，输入应用名称，选择**提交**。

  ![app_register](/img/docs/distribute/app_register.png)

- 登记完成后，即可在应用列表中查看已登记的应用信息。
- 应用开发过程中，需配置应用`app.json`中的`appId`为登记成功的 appId。

  ```json
  {
    "app": {
      "appId": appId
    }
  }
  ```

## 发布应用前提条件

- 您已准备应用的 ZAB 软件包，满足如下要求：
  - 应用名称未被自己开发的其他应用占用。
  - 软件包中的 appId 必须与应用发布时指定的 appId 一致。
- 您需要提前准备如下信息。

  | 准备项         | 说明                                                                                                                                     |
  | -------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
  | 发布国家和地区 | 您需要提前确定应用的发布国家和地区。                                                                                                     |
  | 隐私声明       | 提供此应用的隐私政策文本内容，可帮助用户了解您如何处理敏感的用户数据和设备数据。隐私政策须完整说明您的应用如何收集、使用和分享用户数据。 |

## 配置应用基本信息

- 完成应用登记，并准备好应用 ZAB 软件包，就可以选择您想要发布的应用，提交审核。

  ![app_submit](/img/docs/distribute/app_submit.png)

- 进入应用发布页面，填写应用基本信息，包含上架地区、应用分类、应用安装包、支持设备、版本号、应用语种、应用 icon、隐私声明、调用权限、安装包是否包含 SDK。

  ![app_infomation](/img/docs/distribute/app_infomation.png)

### appId

appId 为应用的唯一标识，在应用登记时自动分配

### 上架地区

请选择您的应用希望上架的国家地区

![app_country](/img/docs/distribute/app_country.png)

### 服务类别

- 普通：无需添加附件；
- 医疗：需上传医疗机构批准书附件
- 保险：需上传保险机构法人许可证、经营保险业务许可证、经营保险经纪业务许可证、经营保险公估业务许可证、经营保险代理业务许可证附件；
- 普通商品销售：需上传 ICP 证（电信与信息服务业务经营许可证）、EDI 证（增值电信业务经营许可证）附件；
- 食品药品保健品及医疗器械销售：需上传食品经营许可证、互联网药品信息服务资质证书、保健食品批准证书、第一类医疗器械生产备案凭证、医疗器械生产许可证、经营许可证附件；

![app_category](/img/docs/distribute/app_category.jpg)

### 应用分类

根据应用的用途，选择对应的分类

![app_category](/img/docs/distribute/app_cate.jpg)

### 开发者

展示您的账号昵称，昵称修改入口为账号中心->账号信息->昵称。昵称修改后再次发起任意提审且审核通过时，将在应用商城更新昵称

### 应用安装包

本地上传应用 ZAB 软件包，该软件包中的 appId 需与当前页面的 appId 一致

### 支持设备

上传应用 ZAB 软件包后，会自动识别填入支持的设备名称

如后续平台检测到开发者的小程序有可支持的新设备，平台将对开发者的小程序主动进行适配并分发至新设备

### 版本号

上传应用 ZAB 软件包后，会自动识别填入当前软件包的版本号

### 应用语种、名称、详细介绍

选择您的应用支持的语种并填写应用名称、应用简介、应用详细介绍、应用介绍预览图

![app_language](/img/docs/distribute/app_language.png)

### 应用介绍截图

- 应用截图的图片输出尺寸为 360×360 px，格式：PNG
- 图片背景保证透明无填充
- 需要保证手表界面在方形的图片区域中最大化展示
- 展示图建议提供3张以上的图片

圆形屏幕：

![app_preview_round](/img/docs/distribute/app_preview_round.png)

- ① 应用界面截图
- ② 360 x 360 px 尺寸的圆形透明背景
- ③ 应用介绍截图：应用界面截图放在方形的透明背景中间，上下左右无边距

方形屏幕：

![app_preview_square](/img/docs/distribute/app_preview_square.png)

- ① 应用界面截图
- ② 360 x 360 px 尺寸的方形透明背景
- ③ 应用介绍截图：应用界面截图放在方形的透明背景中间，上下左右无边距

### 应用 icon

此处的 icon 仅用于在管理中心上传，在应用市场展示

- icon 尺寸大小：240×240 px，图片格式：PNG
- icon 为背景透明的圆形图标，保证四周无填充

![icon_standard](/img/docs/distribute/icon_standard.png)

- ① 应用 icon
- ② 240 * 240 px 尺寸的方形透明背景
- ③ 应用 icon：应用 icon 放在方形的透明背景中间，上下左右无边距

### 隐私声明

请提供此应用的隐私政策文本内容，可帮助用户了解您如何处理敏感的用户数据和设备数据。隐私政策须完整说明您的应用如何收集、使用和分享用户数据。

### 调用权限

勾选应用需要调用的数据权限，若无则勾选“无”

### 安装包是否包含 SDK

若包含 SDK 请描述 SDK 名称及使用目的

## 提交审核

- 所有信息确认无误后，点击**提交审核**按钮发起审核。

  ![app_submit_audit](/img/docs/distribute/app_submit_audit.png)

- 提交成功后，在应用列表中可查看该应用的审核状态，审核时间一般为 1~5 个工作日，请耐心等待。

  ![app_audit_status](/img/docs/distribute/app_audit_status.png)

- 如果审核不通过，可以查看审核不通过原因，选择**编辑**，重新修改。

  ![app_unapproved](/img/docs/distribute/app_unapproved.png)

- 审核通过的应用，还可以升级功能或修复异常，选择**版本升级**，更新版本。

  ![app_approved](/img/docs/distribute/app_approved.png)
