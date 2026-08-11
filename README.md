# 野猪睡眠 AnimalSleep — 法律文件托管（GitHub Pages）

本仓库用于托管 App Store 审核所需的《用户协议》与《隐私政策》。
页面为静态 HTML，中英双语（页面右上角可切换）。

## 文件

- `index.html` — 入口页
- `user-agreement.html` — 用户协议
- `privacy-policy.html` — 隐私政策

## 部署步骤

1. 在 GitHub 新建公开仓库，例如 `animalsleep-legal`。
2. 把以上三个文件上传到仓库根目录。
3. 打开仓库 Settings → Pages。
4. Build and deployment 选择 “Deploy from a branch”，分支选 `main`，目录选 `/ (root)`，点 Save。
5. 等待 1–2 分钟，访问：
   `https://<你的用户名>.github.io/animalsleep-legal/privacy-policy.html`
6. 在 App Store Connect → App 信息 → 隐私政策 URL 填入上面的地址。

## 修改文案

正文同步自 App 内的 LocalizationLegal.swift。需要更新时，重新生成两个 HTML 并
`git commit` 推送即可，GitHub Pages 会自动更新。
