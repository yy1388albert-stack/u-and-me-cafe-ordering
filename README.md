# U & ME CAFÉ 点餐 H5 — GitHub Pages 部署

版本：2026-09-26 导出（当前最新版：英文单语、现金支付、GST 5%、新版首页、手机端地图缩小、地图弹窗只显示店名、地图版权默认收起、电话直拨修复）

## 文件
- `index.html`：单文件版点餐 H5（含全部页面逻辑、样式、菜单数据，开箱即用）

## 部署步骤（2 分钟）
1. 在 GitHub 新建一个仓库（例如 `u-and-me-cafe-ordering`）。
2. 把 `index.html` 上传到仓库根目录（Add file → Upload files）。
3. 仓库 Settings → Pages → Build and deployment → Source 选 **Deploy from a branch**，
   Branch 选 `main`、目录选 `/ (root)`，点 Save。
4. 等 1–2 分钟，访问 `https://你的用户名.github.io/u-and-me-cafe-ordering/` 即可。

## 说明
- 这是纯静态单文件，GitHub Pages 直接可跑；地图、样式 CDN 需要访问者联网。
- 原型内支付/通知为模拟演示，正式上线需接后端、真实支付与通知服务。
- 之后每桌的桌码二维码，编码 `https://你的用户名.github.io/u-and-me-cafe-ordering/?table=桌号` 即可。
