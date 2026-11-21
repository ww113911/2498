[README.md](https://github.com/user-attachments/files/35216906/README.md)
# 语向 · 语言探索手记

当前版本：3.0（2026-11-22）。28 道原创生活情境题、4 个偏好维度、16 种语言。

## 直接打开

用浏览器打开根目录的 `index.html` 即可开始测试。这个文件包含完整 HTML、CSS 和 JavaScript，可离线运行，无需安装依赖。

## 修改与构建

安装 Node.js 18 或更新版本后，在项目根目录运行：

```sh
npm run build
```

构建只使用 Node.js 内置模块，无需运行 npm install。构建会根据源码重新生成根目录 index.html。

| 文件 | 用途 |
| --- | --- |
| index.html | 可直接运行、部署的完整网页 |
| src/data.js | 题目、语言内容和偏好定义 |
| src/app.js | 交互、计分、进度保存和结果卡生成 |
| src/style.css | 页面与手机适配样式 |
| scripts/build.cjs | 生成单文件网页 |
| licenses/feather-MIT.txt | Feather 图标许可 |

上传 GitHub 保存时，将本文件所在目录的全部内容上传到仓库即可。保留 index.html，方便直接取得可运行版本。

## 功能

- 逐题作答、返回修改、自动保存进度。
- 推荐语种、四维偏好解读、特色表达与入门路线。
- 切换其他候选语言、保存 PNG 结果卡、打印报告。
- 手机和桌面布局；不依赖外部字体、图片或脚本。

## 分享地址

当前线上地址：https://compact-flyingfish-d2combcd17593-1387624029.tcloudbaseapp.com/language-compass/?v=3

分享按钮的目标网址在 src/app.js 顶部的 SITE 常量中。迁移网站后请更新该常量，并重新构建。

## 数据与定位

无需登录。答案只在当前浏览器内计算和保存，使用 localStorage 键 language-compass-v3；不会上传或跨设备同步。分享测试网址不含个人答案。

本项目是趣味偏好探索，不是经过验证的心理、语言能力或天赋测评。四维位置与语言入门路线的匹配属于产品设计，不代表使用者的能力或语言群体的性格。

## 版本核对

源码包构建出的 index.html 已与当前交付的 language-compass.html 进行逐字节一致性核对。此前已验证完整答题、修改/恢复进度、16 语种可达、手机布局和结果卡下载。

图标基于 Feather，保留其 MIT 许可；许可也已嵌入构建后的 HTML。
