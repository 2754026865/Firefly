
# Firefly 是使用 Astro 框架构建的现代化、高性能静态博客主题。


[**📝使用文档**](https://docs-firefly.cuteleaf.cn/)

⚡ 静态站点生成: 基于Astro的超快加载速度和SEO优化
🎨 现代化设计: 简洁美观的界面，支持自定义主题色
📱 移动友好: 完美的响应式体验，移动端专项优化
🌟 看板娘支持: 同时支持Spine和Live2D动画引擎，带来丰富的互动体验
🔧 高度可配置: 所有功能模块均可通过配置文件自定义开关和参数

()[firefly.png]

## 👀 要求

- Node.js <= 22
- pnpm <= 9

## 🚀 快速开始

### 📦 安装

1. **克隆仓库：**
   ```bash
   git clone https://github.com/Cuteleaf/Firefly.git
   cd Firefly
   ```

2. **安装依赖：**
   ```bash
   # 如果没有安装 pnpm，先安装
   npm install -g pnpm
   
   # 安装项目依赖
   pnpm install
   ```

3. **配置博客：**
   - 编辑 `src/config.ts` 自定义博客设置
   - 更新站点信息、主题色彩、横幅图片和社交链接
   - 配置特色页面功能

4. **启动开发服务器：**
   ```bash
   pnpm dev
   ```
   博客将在 `http://localhost:4321` 可用


## 📖 配置说明

### 配置文件结构

```
src/
├── config.ts                 # 主配置文件
├── config/
│   ├── adConfig.ts          # 广告配置
│   ├── fontConfig.ts        # 字体配置
│   ├── navBarConfig.ts      # 导航栏配置
│   ├── pioConfig.ts         # 看板娘配置
│   └── sidebarConfig.ts     # 侧边栏配置
└── FooterConfig.html        # 页脚HTML内容
```


## ⚙️ 文章 Frontmatter

```yaml
---
title: My First Blog Post
published: 2023-09-09
description: This is the first post of my new Astro blog.
image: ./cover.jpg
tags: [Foo, Bar]
category: Front-end
draft: false
lang: jp      # 仅当文章语言与 `config.ts` 中的网站语言不同时需要设置
---
```

## 🧞 指令

下列指令均需要在项目根目录执行：

| Command                           | Action                            |
|:----------------------------------|:----------------------------------|
| `pnpm install` 并 `pnpm add sharp` | 安装依赖                              |
| `pnpm dev`                        | 在 `localhost:4321` 启动本地开发服务器      |
| `pnpm build`                      | 构建网站至 `./dist/`                   |
| `pnpm preview`                    | 本地预览已构建的网站                        |
| `pnpm new-post <filename>`        | 创建新文章                             |
| `pnpm astro ...`                  | 执行 `astro add`, `astro check` 等指令 |
| `pnpm astro --help`               | 显示 Astro CLI 帮助                   |


## 📄 许可证

本项目采用 MIT 许可证。详见 [LICENSE](../LICENSE) 文件。

## 🙏 致谢

- 感谢原始 [Fuwari](https://github.com/saicaca/fuwari) 模板
- 感谢基于Fuwari二次开发的[Mizuki](https://github.com/matsuzaka-yuki/Mizuki) 模板
- 使用 [Astro](https://astro.build) 和 [Tailwind CSS](https://tailwindcss.com) 构建
---

如有问题或建议，请提交 [Issue](https://github.com/CuteLeaf/Firefly/issues) 或 [Pull Request](https://github.com/CuteLeaf/Firefly/pulls)。
