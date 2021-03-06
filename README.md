# Read-the-Docs with Github

[![Documentation Status](https://readthedocs.org/projects/zhyantao/badge/?version=latest)](https://zhyantao.readthedocs.io)
[![Repository Size](https://img.shields.io/github/repo-size/zhyantao/zhyantao.github.io)](https://github.com/zhyantao/zhyantao.github.io/archive/refs/heads/master.zip)

## 环境部署

1、在 Github 上创建仓库（仓库名以 `notebook` 为例），创建完成后，克隆 `notebook` 到本地。

```bash
git clone https://github.com/<your_github_username>/notebook.git
```

2、将 [源代码压缩包](https://github.com/zhyantao/readthedocs-with-github/archive/refs/heads/master.zip) 解压后，把压缩包中的内容全部复制到 `notebook` 文件夹中。

3、下载安装 [Graphviz](https://graphviz.org/) 并添加至系统环境变量。安装项目所需依赖。预览效果。

```bash
cd notebook
pip install -r requirements.txt
make html
```

4、提交 `notebook` 仓库的修改到 Github。

```bash
git add . && git commit -m "v1.0.0" && git pull && git push
```

5、登录 [Readthedocs](https://readthedocs.org/) 导入刚刚新建的 Github 项目 `notebook`，构建完成后方可阅读文档。

## 撰写文档

1、把需要发表的文档放在 `notebook/docs` 文件夹中（写作格式可以是 `Markdown` 或者 `reStructuredText` ）

2、打开命令行，并切换到 `notebook` 目录下，输入 `make html`

3、打开 `notebook/build/html/index.html` 预览效果，确认无误后提交代码到 Github 仓库

4、重新打开 [Readthedocs](https://readthedocs.org/) 文档的网址，查看新发表的博客（有延迟，可能需要等待）。

## 注意事项

在 `notebook/docs` 下的添加新文章后需要在 `notebook/docs/index.md` 中添加一条记录。
