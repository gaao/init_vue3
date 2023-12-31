# init_vue3
初始化项目
### 初始化项目
npm init vite@latest project-engineer --template vue-ts
### 安装插件

#### 提供 Vue 3 JSX & TSX 支持（通过 专用的 Babel 转换插件）
npm i -D @vitejs/plugin-vue-jsx
#### 可视化并分析构建包，查看哪些模块占用空间大小，以此来优化构建包的大小
npm i -D rollup-plugin-visualizer

#### 引入 UI 框架：为 ElementPlus 提供按需引入能力
npm i -D vite-plugin-element-plus

### 基于 husky + lint-staged 项目规范化
 #### Eslint
 npm i eslint -D
 ##### 利用 eslint 命令行工具生成基本配置
npx eslint --init
npm i prettier -D
# 带 lint-staged
npm i eslint prettier lint-staged eslint-plugin-prettier eslint-config-prettier -D
# 不带 lint-staged（本文采用方式）
npm i eslint-config-prettier eslint-plugin-prettier -D


# Husky
npm i husky -D
# 生成 .husky 文件夹（注意：这一步操作之前，一定要执行 git init 初始化当前项目仓库，.husky 文件夹才能创建成功）
npx husky-init install

npm i @commitlint/config-conventional @commitlint/cli -D