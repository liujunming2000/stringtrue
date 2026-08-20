# StringTrue 项目文档站 / StringTrue Project Documents

本仓库是 **弦准 (StringTrue)** 应用的公开文档站点，通过 GitHub Pages 托管，用于发布与应用相关的对外文档。

## 已发布页面 / Published pages

| 页面 | 说明 |
|------|------|
| `index.html` | 文档站首页 / 文档目录 |
| `privacy.html` | 隐私政策 / Privacy Policy |
| `license.html` | 软件许可与免责声明 / License & Disclaimer |
| `opensource.html` | 第三方开源组件许可 / Open Source Licenses |

## 线上地址 / Live site

启用 GitHub Pages 后（仓库 Settings → Pages → Source 选 `main` 分支 + `/ (root)`），访问：

```
https://liujunming2000.github.io/stringtrue/
```

各页面链接示例：`https://liujunming2000.github.io/stringtrue/privacy.html`

## 本地预览 / Local preview

直接用浏览器打开 `index.html` 即可；或启动一个本地静态服务器：

```bash
python -m http.server 8000
# 然后访问 http://localhost:8000/
```

## 如何新增文档 / How to add a page

1. 在根目录新增一个 `.html` 文件（如 `help.html`）。
2. 建议沿用统一双语结构：**英文块 → 分隔线 `<hr>` → 中文块**，与现有页面风格一致。
3. 在 `index.html` 的「文档目录」列表中加一行链接：

   ```html
   <li><a href="help.html">使用帮助 / Help</a></li>
   ```

4. 提交并推送到 `main` 分支，GitHub Pages 会自动更新。

## 备注 / Notes

- 本站为独立公开仓库，与 StringTrue 闭源 App 源码仓库互相独立，不暴露任何源码。
- `.nojekyll` 文件用于禁用 GitHub Pages 的 Jekyll 处理，保证 HTML 原样发布。
