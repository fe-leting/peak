# 简介

前端工程化解决方案

## 创建项目

```
fe-peak
```

根据提示进行下一步，直到完成

## 开发

```
yarn start
```

## 编译

```
yarn build
```

## 自定义配置

peak.config.js
```
module.exports = {
  // 开发环境配置
  webpackConfigDev: 'config/webpack.config.dev.js',
  // 生产环境配置
  webpackConfigProd: 'config/webpack.config.prod.js',
  // 模板文件路径
  template: 'index.html',
  // 静态资源目录路径
  publicPath: '/public',
}
```

## 环境变量

会在 window 上注入以下环境变量，环境变量可以在 package.json 中的 script 上设置跟修改

```
window.Peak.env
```

## 代理

```
fetch(`${window.Peak.proxyUrl}http://www.taobao.com`)
```
