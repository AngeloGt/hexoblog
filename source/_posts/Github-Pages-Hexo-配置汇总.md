title: Github Pages + Hexo 安装配置汇总
author: Angelo Guo
date: 2018-10-29 14:29:33
tags:
---
#资源列表
* Git: https://www.git-scm.com/
* Node: https://nodejs.org
* Github: https://github.com/
* Hexo Admin: https://github.com/jaredly/hexo-admin



0. 注册Github
1. 安装Git
2. 安装Node
3. 安装配置Hexo
```
  $ npm install hexo-cli -g
  $ npm install hexo-deployer-git --save
  $ hexo g
  $ hexo d
```
4. 配置ssh
	* ssh -T git@github.com
5. 配置Hexo主题
6. 写Post
	* 安装 Hexo-admin
    ```
npm install --save hexo-admin
hexo server -d
open http://localhost:4000/admin/
    ```
    * 在 http://localhost:4000/admin/ 页面下可以用markdown写文章。