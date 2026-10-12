# AERIAL Lab 主页

AERIAL Lab 实验室的 GitHub Pages 主页。

## 项目信息

- 实验室组织：https://github.com/AERIAL-Lab
- 主页地址：https://aerial-lab.github.io/
- 代码仓库：https://github.com/AERIAL-Lab/aerial-lab.github.io
- 发布配置：https://github.com/AERIAL-Lab/aerial-lab.github.io/settings/pages
- 部署记录：https://github.com/AERIAL-Lab/aerial-lab.github.io/actions

## 当前状态

2026-10-12 完成首次部署，已验证主页返回 HTTP 200，HTTPS 已启用。

已构建简洁学术风格首页，包含实验室实拍首图、中英文介绍、两条研究主线，以及企业合作与学生参与入口。成果、开放课题与联系方式尚待补充，页面未设置虚构的申请或提交功能。本次首页改动的发布状态以 GitHub Pages 部署记录为准。

## 文件结构

- `raw_material/`：实验室原始材料，用于后续生成网页内容与素材；原始文件默认仅本地保存，不随网站发布。
- `index.html`：主页内容与原生折叠交互。
- `styles.css`：桌面与手机响应式样式。
- `assets/aerial-lab-aircraft.jpg`：用户提供的实验室照片，经 JPEG 压缩用于网页。
- `assets/favicon.svg`：网站图标。
- `assets/hfut-logo.png`：合肥工业大学官方校徽与校名组合，保留官网配色。来源：[学校官网标识](https://www.hfut.edu.cn/images/logo-b.png)，参考[工大标识说明](https://www.hfut.edu.cn/xxgk/gdbs.htm)。
- `.nojekyll`：禁用 Jekyll，直接发布静态文件。
- `README.md`：项目说明与发布方式。
- `AGENTS.md`：供后续开发代理使用的维护约定。

## 维护与发布

项目使用原生静态 HTML/CSS，没有构建步骤或依赖安装要求。可直接在浏览器中打开 `index.html`，或在项目目录运行 `python3 -m http.server 8765 --bind 127.0.0.1` 后访问 `http://127.0.0.1:8765/` 预览。

GitHub Pages 从 `main` 分支的仓库根目录 `/` 发布。修改完成后，提交并推送到 `main`，GitHub 会自动运行 `pages build and deployment` 工作流。

发布后检查部署记录，并访问主页确认变更生效。不要将密钥、凭据或内部资料放入仓库；仓库及站点均为公开内容。
