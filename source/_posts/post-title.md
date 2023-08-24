---
title: post title
tags:
  - '图片'
categories:
  - '头像'
date: 2023-08-17 11:58:00
---
## 应用介绍

* [ ] 有菜单权限就有页面的访问权限（后端无需校验）
* [ ] 系统子应用，查询application表
* [ ] 待审核

> 头像

![头像](https://cdn.dukedream.top/wallhaven.png)

> 头像2

![头像2](https://cdn.dukedream.top/jm.png)

```mermaid
stateDiagram-v2
    direction LR
    [*] --> 待审核 : 新增
    待审核 --> 未展示 : pass
    未展示 --> 展示中 : 上架
    展示中 --> 未展示 : 下架
    未展示 --> [*] : 删除
    待审核 --> 审核不通过 : no pass
    审核不通过 --> 待审核 : 编辑
    审核不通过 --> [*] : 删除
```

> 666