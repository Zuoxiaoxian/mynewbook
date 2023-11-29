---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Notebooks with MyST Markdown

Jupyter Book还允许您使用MyST Markdown编写基于文本的笔记本。
看 [带有MyST Markdown文档的笔记本](https://jupyterbook.org/file-types/myst-notebooks.html) 了解更多详细说明。
这个页面展示了一个用MyST Markdown写的笔记本。

## An example cell

使用MyST Markdown，您可以使用如下指令定义代码单元：

```{code-cell}
print(2 + 2)
```

当你的书被构建时，任何 `{code-cell}` 块的内容都将是
使用默认的Jupyter内核执行，并且将显示它们的输出
与其他内容保持一致。

```{seealso}
Jupyter Book使用 [Jupytext](https://jupytext.readthedocs.io/en/latest/) to convert text-based files to notebooks, and can support [许多其他基于文本的笔记本文件](https://jupyterbook.org/file-types/jupytext.html).
```

## Create a notebook with MyST Markdown

MyST Markdown笔记本由两个方面定义：

1. YAML metadata that is needed to understand if / how it should convert text files to notebooks (including information about the kernel needed).
   See the YAML at the top of this page for example.
2. The presence of `{code-cell}` directives, which will be executed with your book.

这就是开始所需的全部内容！

## Quickly add YAML metadata for MyST Notebooks

如果您有一个markdown文件，并且希望快速向其中添加YAML元数据，以便Jupyter Book将其视为MyST markdown Notebook，请运行以下命令：

```
jupyter-book myst init path/to/markdownfile.md
```
