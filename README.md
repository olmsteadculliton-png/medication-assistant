# 安心用药 Web 原型

手机样式的用药助手交互 Demo。入口为 `prototype/index.html`。

支持同时间段药品合并、整组确认/跳过/稍后提醒、计划编辑、药品类型匹配与疗程计算、老人/亲属视角和历史记录。

当前数据保存在浏览器 localStorage，未连接线上数据库。身份切换和 OCR 为演示；不同设备不会同步。仅使用模拟药品数据。

## 本地访问
在 prototype 目录运行 `python -m http.server 5173 --bind 127.0.0.1`，访问 http://127.0.0.1:5173/ 。

## GitHub Pages
将本项目推送到仓库 main 分支后，在 Settings → Pages → Build and deployment 选择 GitHub Actions。仓库已有自动发布工作流，只发布 prototype 目录。

在 Actions 查看 Publish Web prototype；成功后从 github-pages 环境读取实际网页链接。后续 main 分支更新自动重新发布。

架构与云端开发计划见 docs/开发方案.md。
