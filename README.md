# 同频 · 展厅相遇 — 现场试用 MVP

这是一个适用于静态 HTTPS 托管的双人互动页面。访客用一台手机轮流操作：第一位选择自己的观展起点，第二位先猜、再选择自己的习惯；系统揭晓差异并给出一条面对面聊天提示。

## GitHub Pages 发布

1. 把本目录内容放到目标仓库根目录（包括 `.github/workflows/deploy.yml` 和 `.nojekyll`）。
2. 在仓库 Settings → Pages → Build and deployment，将 Source 设为 **GitHub Actions**。
3. 将文件推到 `main` 分支，工作流会自动部署。

页面预期地址：`https://zhuangwenwen454-png.github.io/jiao/`。

## 入口二维码地址

发布后可为不同入口制作二维码，编码以下页面地址：

- 展厅入口：`https://zhuangwenwen454-png.github.io/jiao/?source=entrance-A1`
- 休息区：`https://zhuangwenwen454-png.github.io/jiao/?source=lounge-B1`
- 活动区：`https://zhuangwenwen454-png.github.io/jiao/?source=event-C1`

请在 Pages 部署成功并确认地址可访问后，再生成现场二维码。

## 数据说明

匿名行为记录需由访客自愿勾选授权。当前版本把记录保存在本机浏览器，可在“研究视图”导出 CSV；不同访客手机之间不会自动汇总。适合先用一台共用手机或平板做小规模现场观察。若要让每位访客用自己的手机并汇总到同一份研究数据，需要再接入一个匿名事件 API。

无需登录、麦克风、摄像头或作品端传感器；页面无外部脚本依赖。