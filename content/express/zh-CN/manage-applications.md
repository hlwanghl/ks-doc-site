---
title: "应用模板"
---

应用模板相当于 Helm 应用仓库中的 chart 模板，通过可视化的方式在 KubeSphere 中展示并提供部署及管理功能，用户可以基于应用模板快速地一键部署应用。

## 部署应用

参考 [添加应用仓库说明](/express/zh-CN/manage-repo) 来添加应用仓库，KubeSphere 会自动加载此仓库下的所有应用。在左侧菜单栏 **应用管理** 菜单下，点击 **应用模板** 按钮进入列表页。注意：默认会将来自所有仓库的应用模板都列出来，可以通过左上角的下拉框进行来源过滤。

![应用模版列表](/apptemplates_list.png)

1. 找到所需的应用，点击 **应用详情** 按钮。

2. 弹出窗口左侧为当前应用的详细信息和说明文档，右侧为需要填写的和部署相关的参数。

> - 名称：为所部署应用命名，如不填，则自动生成一个随机名称
> - 版本：选择所需应用版本
> - 项目：选择应用部署的目标项目
> - 描述信息：关于被部署应用的一些详细信息
> - 配置参数：以可视化的方式，将 Helm Chart 应用包中的 values.yaml 展示出来，里面包含了应用开发者允许用户自定义的参数，用户可以根据实际情况进行填写

![应用模版详情页](/apptemplate_deploy.png)

3. 点击右上角 **代码模式** 按钮，可以查看当前应用中的所有文件的详细内容。

![应用模版 - 代码模式](/apptemplates_yaml.png)

4. 当所需参数输入完成后，点击 **部署** 按钮进行部署，用户可以在相关工作负载菜单下查看部署进展情况。
