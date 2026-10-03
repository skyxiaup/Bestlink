# Bestlink Website

BestLink (bestlinktec.com) 官网 - 工业网络设备供应商，主营 PoE 交换机、光纤收发器、Type-C Hub 等产品。

## 项目结构

```
Bestlink/
├── index.html          # 首页
├── products.html      # 产品列表
├── catalog.html       # 产品目录
├── about.html         # 关于我们
├── service.html       # 服务支持
├── solution.html      # 解决方案
├── contact.html       # 联系我们
├── demo.html          # Demo 页面
├── logo.png           # Logo
├── images/            # 产品图片
│   └── products/      # 各产品图片
├── wp-content/        # WordPress 上传资源（参考用）
└── CLAUDE.md         # 本文件
```

## 技术架构

- **纯静态 HTML** + 内联 CSS/JS（无外部样式表）
- CSS/JS 全部内联在 HTML 中
- 图片存储在 `images/` 目录
- WordPress `wp-content/uploads/` 中的图片已下载本地备份

## 迁移计划

将重构为 **Astro 静态站点**，好处：
- Markdown 管理产品内容
- 自动化 SEO（meta + sitemap）
- 产品页面模板化（新增产品只需加 .md 文件）
- GitHub Actions 自动部署

## 部署

- **当前**: SiteGround FTP 手动上传
- **目标**: GitHub + GitHub Actions 自动 SFTP 部署

## 设计参考

- 品牌色: `#00162f` (深蓝), `#00c961` (绿色)
- 字体: Segoe UI, Arial, sans-serif
- 产品: PoE 交换机、光纤收发器、Type-C Hub

## 站点分析

- IP: 35.213.130.103
- FTP Host: 35.213.130.103 (需用 IP，域名解析失败)
- FTP User: openclaw@bestlinktec.com
