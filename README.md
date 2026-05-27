# marp-theme-tongji

## 项目简介
本仓库提供一个为 Marp 制作的「同济」风格幻灯片主题（CSS），并附带示例源码与导出示例，适用于教学、报告与学术演示。

## 主要特性
- 同济视觉风格的配色与章节页样式
- 支持 LaTeX 数学公式、代码高亮与常见 Marp 布局

## 快速开始
1. 克隆仓库：

```
git clone https://github.com/Double-Cloth/marp-theme-tongji.git
cd marp-theme-tongji
```

2. 本仓库的示例文件位于 `src/`，常用路径：

- 示例 Markdown： `src/demo.md`
- 主题 CSS： `src/themes/tongji.css`
- 图片资源： `src/images/assets/`
- 导出示例： `export/demo.html`

3. 在本地预览（推荐）：

- 安装 VS Code 扩展 `Marp for VS Code`，打开 [src/demo.md](src/demo.md) 并使用扩展的预览/导出功能。

4. 使用 Marp CLI 导出 HTML（示例命令）：

```
npx @marp-team/marp-cli src/demo.md -o export/demo.html --theme src/themes/tongji.css
```

## 项目结构（主要文件/目录）
- `src/demo.md` — 示例幻灯片 Markdown（含 front-matter）
- `src/themes/tongji.css` — 主题样式（可直接在 Marp 中引用）
- `src/images/assets/` — 主题使用的图片资源和背景图
- `export/` — 导出后的示例文件（如 `export/demo.html`）

## 如何自定义
- 修改主题：编辑 `src/themes/tongji.css` 来调整颜色、字体和背景。
- 修改示例：编辑 `src/demo.md` 来调整内容、分隔与布局。
- 替换图片：把图片放入 `src/images/assets/`，并在 CSS/Markdown 中使用相对路径引用。

## 其他
- 若需导出为 PPTX，可使用支持 PPTX 导出的 Marp 工具链或在线转换（注意不同导出器对样式的支持程度可能不同）。
- 将常用导出命令写入 npm script 以便统一使用。
