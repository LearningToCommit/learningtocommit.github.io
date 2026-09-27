# Learning to Commit project page

独立的论文项目主页，可直接交给 GitHub Pages 托管，无需安装依赖或构建。所有研究内容来自提供的论文正文，未使用代码实现、内部文档、审稿材料或附录扩展内容。

## 本地查看

在本目录运行 `python3 -m http.server 8765`，然后打开 http://localhost:8765 。也可以直接打开 `index.html`。在线字体不可用时会使用系统字体。

## 发布到组织主页

将本目录文件放入 `LearningToCommit/learningtocommit.github.io` 仓库，在仓库 Settings → Pages 中选择从 `main` 分支根目录发布。最终地址为 https://learningtocommit.github.io/ 。发布前应核对论文和作者信息是否为希望公开的版本。

## 内容来源

源论文：作者提供的 Learning to Commit 稿件，本页使用 2026-09-27 提供的版本。

- 标题与作者：`main.tex` 中启用的作者块，已与 `main.pdf` 首页核对。
- 概念、方法、评估维度：`sections/00_abstract.tex`、`sections/01_introduction.tex`、`sections/03_methodology.tex`。
- 主基准数字、方法对比和学习曲线：`sections/04a_experiments_organic.tex`，表 `tab:main_results`、图 `fig:convergence`。
- SWE-bench Pro：`sections/04b_experiments_swe.tex`，表 `tab:swebench_pro`。明确标注 50 道抽样任务及 4 次独立运行，不作为全榜成绩。
- `assets/paper.pdf` 是原始 `main.pdf` 的副本。两张网页配图由正文引用的 `figures/framework_final.pdf` 和 `figures/organic_eval/convergence.pdf` 转成 PNG，未修改数据。
- BibTeX 按作者确认，使用当前投稿版标题和作者名单，沿用原 arXiv 条目的编号 `2603.26664`、年份、分类和链接；arXiv 更新版本后仍使用同一编号。
- GitHub 按钮链接到已存在的组织主页，不声称代码已发布。

修改文字和布局用 `index.html`，样式用 `styles.css`，步骤切换和实验表数据用 `script.js`。
