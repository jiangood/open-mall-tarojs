# Open Mall Taro.js

## 项目介绍

Open Mall Taro.js 是一个基于 Taro.js 开发的多端电商小程序项目，支持微信小程序、支付宝小程序、H5 等多个平台。项目采用 React 框架和 Less 样式，提供了完整的电商购物流程。

## 技术栈

- **框架**: Taro.js 4.1.11
- **前端**: React 18.0.0+、Less
- **样式风格**: 有赞风（红色系列）
- **构建工具**: Webpack 5.91.0
- **代码规范**: ESLint、Stylelint

### 有赞常用颜色

| 颜色名称 | 颜色值 | 用途 |
|---------|-------|------|
| 主红色 | #FF4444 | 主要按钮、价格、重要信息 |
| 辅助红色 | #FF6666 | 次要按钮、提示信息 |
| 背景色 | #F5F5F5 | 页面背景 |
| 卡片背景 | #FFFFFF | 卡片、容器背景 |
| 主文字 | #333333 | 标题、重要文字 |
| 次要文字 | #666666 | 正文、描述文字 |
| 辅助文字 | #999999 | 辅助信息、提示文字 |
| 边框颜色 | #E5E5E5 | 边框、分割线 |

## 目录结构

```
├── config/            # 项目配置文件
│   ├── dev.js         # 开发环境配置
│   ├── index.js       # 主配置文件
│   └── prod.js        # 生产环境配置
├── src/               # 源代码目录
│   ├── components/    # 公共组件
│   ├── pages/         # 页面
│   ├── services/      # 数据服务
│   ├── app.config.js  # 应用配置
│   ├── app.js         # 应用入口
│   └── app.less       # 全局样式
├── .editorconfig      # 编辑器配置
├── .env.development   # 开发环境变量
├── .env.production    # 生产环境变量
├── .env.test          # 测试环境变量
├── .eslintrc          # ESLint 配置
├── .gitignore         # Git 忽略文件
├── babel.config.js    # Babel 配置
├── commitlint.config.mjs  # Commitlint 配置
├── package-lock.json  # 依赖锁文件
├── package.json       # 项目依赖
├── project.config.json  # 项目配置
└── stylelint.config.mjs  # Stylelint 配置
```

## 功能模块

### 1. 首页
- 轮播图展示
- 分类导航
- 热门商品推荐
- 搜索功能

### 2. 分类页
- 商品分类展示
- 分类商品列表

### 3. 商品详情页
- 商品信息展示
- 商品规格选择
- 加入购物车
- 立即购买

### 4. 购物车
- 商品列表管理
- 商品数量调整
- 商品删除
- 结算功能

### 5. 个人中心
- 用户信息展示
- 订单管理
- 地址管理
- 收藏夹

### 6. 搜索页
- 关键词搜索
- 搜索历史
- 热门搜索

### 7. Tabbar 导航
- 自定义底部导航栏
- 包含首页、分类、购物车、我的四个标签页
- 支持标签页切换和页面跳转

## 数据服务

项目的数据服务统一放在 `services` 目录下，包含以下模块：



**说明**：项目目前使用模拟数据进行开发和测试，实际部署时需要替换为真实的 API 接口。



### 构建生产版本

#### 微信小程序

```bash
npm run build:weapp
```

#### H5

```bash
npm run build:h5
```



## 注意事项

数据服务统一放在 services 目录

测试时使用 `build:h5` 命令

禁止使用 await，优先使用 Promise

