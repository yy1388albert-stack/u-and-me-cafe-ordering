# U & ME CAFÉ — Ordering prototype

Muse 导出的静态点餐演示。无需安装依赖、构建或数据库；直接打开 index.html 即可预览。

## 演示范围与限制
- 菜单、规格、购物车、堂食桌号、外带和配送流程，以及中英法界面切换。
- 订单仅存在当前页面内存中；刷新即丢失，不会发送给餐馆，也不能跨设备同步。
- 支付、短信/邮件通知、会员及订单状态推进均为演示；没有真实支付或商家后台。
- 金额逻辑为原型示意，未实现税费计算；不用于真实结账。
- 地图依赖 unpkg.com 的 MapLibre GL 5.23.0 及 tiles.openfreemap.org；地图失败时隐藏地图。
- 请勿在演示中输入真实客户资料。

## 本地运行
直接双击 index.html，或通过任意静态 HTTP 服务器打开。没有 npm install / build 步骤。

## GitHub Pages
在仓库 Settings → Pages 中选择 Deploy from a branch，main 分支和 / (root)，保存。
预期地址：https://yy1388albert-stack.github.io/u-and-me-cafe-ordering/
桌号示例：在网址后加 ?table=A01，然后选择堂食。
.nojekyll 禁用 Jekyll 处理。后续提交 main 后由 Pages 自动更新。

GitHub Pages 仅用于本项目原型展示。正式商业点餐服务需要其他运行平台、数据库、商家身份验证及订单 API。
官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits

## 文件
- index.html：应用、样式、菜单和内嵌图片。
- .gitignore：排除环境变量、密钥、缓存和开发产物。
- .nojekyll：静态发布标记。

## 安全与维护
本次导出没有发现常见密钥格式或凭证配置；这不等于完整安全审计。
不要在前端源码中加入私钥或数据库密码。未来后端密钥应由服务端环境变量管理。
未添加开源许可证；图片、品牌和菜单内容沿用原始导出。
