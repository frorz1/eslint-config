# 简介
`common-eslint-config` 通用的前端 Lint 规范解决方案。通过对社区开源的各类 Lint 方案进行层叠配置，提供前端技术栈的 Lint 规范。

# 安装
```
npm install @frorz/common-eslint-config --save-dev
```

# 配置
## 配置示例
基础配置
```
{
  "extends": "@frorz/common-eslint-config"
}
```
`common-eslint-config` 提供多种 eslint-config 配置，可以灵活根据项目技术栈进行配置。
```
{
  "extends": "@frorz/common-eslint-config/eslintrc.react.js"
}
```
`or`
```
module.exports = {
  extends: [
    '@frorz/common-eslint-config',
    'plugin:prettier/recommended',
  ],
}
```
## 配置选项
| 选项 | 介绍 | npm包
| --- | --- | ---
| eslintrc.base.js | 约定统一的 js 语法和格式规范，所有规则集都基于此扩展 | `eslint-config-standard`
| eslintrc.react.js | 提供对 react 框架的代码规范支持 | `eslint-plugin-react`
| eslintrc.rn.js | 提供对 react-native 框架的代码规范支持 | `eslint-plugin-react-native`
| eslintrc.ts.js | 提供对 typescript 的代码规范支持 | `@typescript-eslint/eslint-plugin`
| eslintrc.react-ts.js | 提供 react + typescript 的代码规范支持 | `eslint-plugin-react` `@typescript-eslint/eslint-plugin`
| eslintrc.rn-ts.js | 提供 rn + typescript 的代码规范支持 | `eslint-plugin-react-native` `@typescript-eslint/eslint-plugin`

## 其他配置
如果你想修改或者添加 `common-eslint-config` 提供的默认规则，可以直接在工程的 `eslintrc` 文件中进行覆盖配置。

