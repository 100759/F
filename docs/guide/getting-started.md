# 快速开始

## 安装

首先，确保你的系统已经安装了 Node.js 16 或更高版本。

## 创建项目

1. 创建并进入一个新目录：

```bash
mkdir my-docs
cd my-docs
```

2. 初始化项目：

```bash
npm init -y
```

3. 安装 VitePress：

```bash
npm install -D vitepress
```

## 配置项目

1. 创建文档目录：

```bash
mkdir docs
```

2. 创建配置文件：

```bash
mkdir docs/.vitepress
```

3. 在 `docs/.vitepress/config.ts` 中添加基本配置：

```ts
import { defineConfig } from 'vitepress'

export default defineConfig({
  title: "我的文档",
  description: "使用 VitePress 创建的文档",
})
```

## 启动开发服务器

在 `package.json` 中添加以下脚本：

```json
{
  "scripts": {
    "docs:dev": "vitepress dev docs",
    "docs:build": "vitepress build docs",
    "docs:preview": "vitepress preview docs"
  }
}
```

然后运行：

```bash
npm run docs:dev
```

现在你可以在浏览器中访问 `http://localhost:5173` 查看你的文档网站了！ 