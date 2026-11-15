# 欲蓝财务 · 官网主页

线上站点： https://yulancloud.us.ci/

基于 PHP + SQLite 商城系统的产品官网单页，视觉与商城前台同源（复用 `assets/style.css` 的 CSS 变量与组件类），
支持亮色/暗色主题切换与移动端响应式。纯静态、无构建步骤，GitHub Pages 直接托管 main 分支根目录。

## 文件

| 文件 | 说明 |
| --- | --- |
| `index.html` | 主页单页（顶栏 / 首屏 / 功能 / 交付流程 / 文档 / 下载 / 部署 / 页脚） |
| `assets/style.css` | 视觉底座，与商城 `public/assets/style.css` 同源 |
| `assets/home.css` | 官网独有区块样式，全部复用商城 CSS 变量 |
| `assets/favicon.svg` | 站点图标 |
| `CNAME` | 自定义域名 `yulancloud.us.ci`，请勿删除 |
| `404.html` | SPA/深链兜底（复制首页） |
| `.nojekyll` | 禁用 Jekyll 处理 |

## 自定义域名

DNS（Cloudflare）需为根域添加 4 条 A 记录，均设为 **DNS only（灰云）**：

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

仓库 `Settings → Pages → Custom domain` 填 `yulancloud.us.ci`。灰云是 GitHub 签发/续期
Let's Encrypt 证书的前提；橙云会返回 Cloudflare IP，导致证书签不出来。

## 相关链接

- 文档站： https://doc.yulancloud.us.ci/
- 主仓库（系统源码 / 系统包）： https://github.com/yulancloud/yulancloud
- Windows APP 仓库（exe）： https://github.com/yulancloud/yulancloudRubik-Windows
- 文档仓库： https://github.com/yulancloud/doc
