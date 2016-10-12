---
title: Github Page 搭建的某些坑
date: 2016-10-11 11:51:25
tags: Git
---



* 建立 `username` 同名仓库，否则会造成使用 `username.github.io` 访问404错误

* Git的默认安装方式因为添加到PATH的路径的原因，会造成后面hexo deploy的命令不能在Cmd底下运行，在Git Bash底下运行正常

* _config.yml 中配置你所要部署的站点(注意:后面有个空格)
```
# Deployment
## Docs: https://hexo.io/docs/deployment.html
deploy:
  type: git
  repo: git@github.com:<username>/<username>.github.io.git
  branch: master
```