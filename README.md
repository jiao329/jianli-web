# 简历工坊

一个无需后端的在线简历编辑工作台，支持：

- 个人信息、简介、工作经历、教育经历、技能与项目编辑
- 工作经历动态添加 / 删除
- 经典、现代、紧凑三种版式和五种主题色
- 自动保存到浏览器 `localStorage`
- 系统打印导出 PDF、画布导出 PNG、分享链接复制
- 桌面端双栏编辑，移动端纵向预览

## 本地运行

项目是静态页面，可直接使用任意静态服务器打开：

```bash
python -m http.server 4173
```

然后访问 `http://127.0.0.1:4173`。

## Git 历史

当前执行环境禁止写入默认 `.git` 目录，因此提交记录保存在项目内的 `git-records` 目录。查看历史：

```bash
git --git-dir=git-records --work-tree=. log --oneline
git --git-dir=git-records --work-tree=. status
```
