# Mkdocs
## 简介
MkDocs 是一个快速、简单的静态站点生成器，用于构建项目文档。它使用 Markdown 语言编写文档，并使用 MkDocs 配置文件来定义站点结构和样式。
## 简单使用
- 创建一个新的 MkDocs 项目，可以使用命令 `mkdocs new <project_name>`
- 进入项目目录，使用命令 `mkdocs serve` 启动本地服务器，然后在浏览器中访问 `http://127.0.0.1:8000` 查看文档
- （由于ZJU git自带渲染，故这个不需要，可以阅读：[ZJU Git Pages使用指南](https://www.pages.zjusct.io/posts/zju-git-pages/#%E8%87%AA%E5%BB%BA-ci-%E7%9A%84%E9%A1%B5%E9%9D%A2%E7%94%9F%E6%88%90%E5%99%A8%E4%BB%A5-mkdocs-%E4%B8%BA%E4%BE%8B){:target="_blank"}）使用命令 `mkdocs build` 构建文档，生成的静态文件将保存在 `site` 目录中
## 文件结构
- `mkdocs.yml`：MkDocs 配置文件，定义了站点结构和样式
- `docs` 目录：存放 Markdown 文档的目录
- `site` 目录：存放构建后的静态文件的目录（本站不需要）