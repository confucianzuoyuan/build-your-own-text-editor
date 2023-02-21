# 构建你自己的文本编辑器

欢迎！这是一本说明手册，向你展示如何使用 `C` 语言构建终端（Terminal）的文本编辑器。

我们的文本编辑器在 antirez[^1] 的 kilo 的基础上有一些修改。它在单个文件中包含大约 1000 行 `C` 语言代码，没有依赖项，它实现了你在最小编辑器中期望的所有基本功能，以及语法高亮显示和文本搜索功能。

这本小册子将分 184 个步骤来带你构建一个文本编辑器。每一步，你都将添加、更改或删除几行代码。大多数步骤，你都可以通过立即编译和运行程序来观察所做的更改。

我会解释整个过程中的每一步，有时会非常详细。可以随意浏览或者跳过我的说明，因为本文的要点是你将从头开始构建文本编辑器！沿途学到的任何东西都是额外的收获，只需输入代码的更改并观察结果，就可以学到很多东西。

如果你已经准备好开始，请转到第 [1](https://confucianzuoyuan.github.io/build-your-own-text-editor/#_%E8%AE%BE%E7%BD%AE) 章！

**目录**

1. [设置](https://confucianzuoyuan.github.io/build-your-own-text-editor/#_%E8%AE%BE%E7%BD%AE)
2. [进入原始模式](https://confucianzuoyuan.github.io/build-your-own-text-editor/#_%E8%BF%9B%E5%85%A5%E5%8E%9F%E5%A7%8B%E6%A8%A1%E5%BC%8F)
3. [原始输入和输出](https://confucianzuoyuan.github.io/build-your-own-text-editor/#_%E5%8E%9F%E5%A7%8B%E8%BE%93%E5%85%A5%E4%B8%8E%E8%BE%93%E5%87%BA)
4. [文本查看器](https://confucianzuoyuan.github.io/build-your-own-text-editor/#_%E6%96%87%E6%9C%AC%E9%98%85%E8%AF%BB%E5%99%A8)
5. 文本编辑器
6. 搜索
7. 语法高亮

[^1]: redis作者