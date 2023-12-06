# Markdown Files

无论您是用Jupyter Notebooks(`.ipynb`)还是
在常规markdown文件(`.md`)中，您将使用相同风格的markdown进行编写
名为**MyST Markdown**。
这是一个简单的文件，可以帮助您入门并展示一些语法。

## What is MyST?

MyST代表“标记结构化文本”。它
是一种叫做"CommonMark"降价的降价风格的轻微变体，
使用小的语法扩展，允许您编写**角色**和**指令**
在狮身人面像生态系统中。

For more about MyST, see [the MyST Markdown Overview](https://jupyterbook.org/content/myst.html).

## Sample Roles and Directives

Roles and directives are two of the most powerful tools in Jupyter Book. They
are kind of like functions, but written in a markup language. They both
serve a similar purpose, but **roles are written in one line**, whereas
**directives span many lines**. They both accept different kinds of inputs,
and what they do with those inputs depends on the specific role or directive
that is being called.

Here is a "note" directive:

```{note}
Here is a note
```

当你构建你的书时，它会被呈现在一个特殊的盒子里。

Here is an inline directive to refer to a document: {doc}`markdown-notebooks`.


## Citations

You can also cite references that are stored in a `bibtex` file. For example,
the following syntax: `` {cite}`holdgraf_evidence_2014` `` will render like
this: {cite}`holdgraf_evidence_2014`.

Moreover, you can insert a bibliography into your page with this syntax:
The `{bibliography}` directive must be used for all the `{cite}` roles to
render properly.
For example, if the references for your book are stored in `references.bib`,
then the bibliography is inserted with:

```{bibliography}
```

## Learn more

This is just a simple starter to get you started.
You can learn a lot more at [jupyterbook.org](https://jupyterbook.org).
