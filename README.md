这是一个基于 AI 的研究助手应用程序,它通过结合搜索引擎、网页抓取和大型语言模型,能够对任何主题进行迭代式的深入研究。

## 项目技术栈

- Vue.js
- TypeScript
- JavaScript

## docker 部署

```bash
docker run -p 3000:3000 --name deep-research-web -d anotia/deep-research-web:latest

#  浏览器输入：localhost:3000
docker build -t deep-research-web .
docker run -p 3000:3000 --name deep-research-web -d deep-research-web
```


## 安装

```bash
# MAC OS安装 pnpm
brew install pnpm

# 安装依赖
pnpm install

# 1. 开发环境下部署
pnpm dev

# 2. 生成环境下部署SSR应用
pnpm build 

# 3. 生产环境下部署SSG模式
pnpm generate

# 4. 生产环境下本地预览
pnpm preview
```