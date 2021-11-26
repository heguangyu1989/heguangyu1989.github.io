---
title: "Go使用本地项目"
date: 2021-11-26T15:01:10+08:00
draft: true
---


## 核心步骤
1. 初始化一个需要被其他项目引用的项目. eg: ` go mod init git-pri.pri.com/test/modx `
2. 修改git默认使用ssh方式: `git config --global url.ssh://git@git-pri.pri.com/.insteadOf https://git-pri.pri.com/ `
3. 配置go env : `go env -w GOPRIVATE=git-pri.pri.com`
