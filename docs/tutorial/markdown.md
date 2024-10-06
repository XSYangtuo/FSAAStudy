# Markdown

## Markdown简介
Markdown是一种轻量级标记语言，它允许人们使用易读易写的**纯文本格式**编写文档，然后转换成有效的文档。Markdown的目标是实现「易读易写」。Markdown文件的后缀为`.md`。
## 一些简单的Markdown语法
### 标题
=== "代码"
    ```markdown
    # 一级标题
    ## 二级标题
    ### 三级标题
    ```
=== "效果"
    # 一级标题
    ## 二级标题
    ### 三级标题
### 引用
=== "代码"
    ```markdown
    > 这是一个引用
    ```
=== "效果"
    > 这是一个引用
### 强调
=== "代码"

    ```markdown
    *斜体*
    **粗体**
    ```
=== "效果"

    *斜体*  
    **粗体**

### 列表
=== "代码"
    ```markdown
    - 无序列表
    - 无序列表
    ```
=== "效果"
    - 无序列表
    - 无序列表
### 链接
=== "代码"
    ```markdown
    - [百度，不新建标签页](https://www.baidu.com)
    - [百度，新建标签页](https://www.baidu.com){:target="_blank"}
    ```
=== "效果"
    - [百度，不新建标签页](https://www.baidu.com)
    - [百度，新建标签页](https://www.baidu.com){:target="_blank"}
### 其他
你可以阅读[Markdown语法 - 菜鸟教程](https://www.runoob.com/markdown/md-tutorial.html)来了解更多语法。
## Material for Mkdocs拓展的一些使用
完全的扩展可以查看[material for Mkdocs](https://squidfunk.github.io/mkdocs-material/reference/)
### 按钮
=== "代码"
    ```markdown
    [百度](https://www.baidu.com){ .md-button }
    [百度](https://www.baidu.com){ .md-button .md-button--primary }
    ```
=== "效果"
    [百度](https://www.baidu.com){ .md-button }
    [百度](https://www.baidu.com){ .md-button .md-button--primary }
### tab
=== "代码"
    ```markdown
    === "Tab1"
        内容1
    === "Tab2"
        内容2
    ```
=== "效果"
    === "Tab1"
        内容1
    === "Tab2"
        内容2
!!! warning
    tab的标题不能为空，否则会报错,而且tab下方的内容对制表符敏感，请确保每一行都缩进4个空格。
### 提示块
=== "代码"

    ```markdown
    !!! note
        这是一个提示块
    !!! warning
        这是一个警告块
    !!! quote
        这是一个引用块
    ```
=== "效果"

    !!! note
        这是一个提示块
    !!! warning 
        这是一个警告块
    !!! quote
        这是一个引用块
