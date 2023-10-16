# @aaron-zon/prettier-config[![npm](https://img.shields.io/npm/v/@aaron-zon/prettier-config.svg)](https://www.npmjs.com/package/@aaron-zon/prettier-config)

Prettier config.
Prettier是进行代码美化的一种方式
使用此配置包可以让代码根据编辑的规则进行美化

- 单行最大文字数 120
- tab填充空格数 4 
- 结尾添加分号
- 使用单引号
- jsx使用单引号
- 对象中括号与文字之间填充空格
- 标签多行时结尾>换行
- 箭头函数 参数在唯一时也包含在括号中

## 安装

```bash
npm i -D prettier @aaron-zon/prettier-config

or

pnpm i -D prettier @aaron-zon/prettier-config
```

在项目的package.json中添加以下属性
```json
"prettier": "@aaron-zon/prettier-config"
```

## 使用手动美化

1.在项目package.json的scripts中写入新的命令
```json
"lint": "prettier --write  \"src/**/*.{js,ts,json,tsx,css,less,scss,vue,html,md}\""
```

2.在需要进行代码美化的时机执行此命令
```bash
npm run lint
```

## 使用自动美化
1.在项目根目录 .vscode 文件夹下创建settings.json文件

2.在settings.json中写入以下内容
```json
{
    "editor.formatOnSave": true
}
```

3.在编写代码后进行保存ctrl + s，代码会自动进行美化


## 参考

- https://github.com/sxzz/prettier-config

