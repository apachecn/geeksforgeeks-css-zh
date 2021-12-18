# 为什么要创建 SASS 缓存文件夹？

> 原文:[https://www . geesforgeks . org/为什么-sass-cache-folder-is-created/](https://www.geeksforgeeks.org/why-does-sass-cache-folder-is-created/)

CSS 用于设计网页的样式，并且通常改善网页的用户界面和体验。这种 CSS 设计模板的开发包括为 CSS 制作资源，然后编写代码，之后进行测试。测试包括在执行程序之前对其进行编译。CSS 资源和代码的这种编译可能会占用一些时间。

**SASS 和缓存文件夹:** **Sass** 是一个 CSS **预处理器**，完全兼容 CSS 的每个版本。Sass 减少了 CSS 的重复，因此节省了编写 CSS 代码的时间。

引入 SASS 缓存文件夹是为了减少开发和测试 CSS 程序时多次编译和重新编译所花费的时间。当模板的部分在之前的编译过程中没有改变时，当前的模板可以被编译和缓存。在重新编译期间，与上次编译相比，从编译期间未更改的模板部分的缓存文件中加载这些先前编译的数据花费的时间更少。

**缓存文件夹的工作方式:**这个 SASS 文件夹将部分和模板缓存在**块**中。在重新编译模板时，系统将这些缓存的块与正在编译的新模板进行比较，并且系统只重新编译模板中已经进行了更改的部分。模板的其余未更改部分不需要再次重新编译，因为系统将只使用缓存的先前编译的部分，并将其复制过来以创建新的编译文件，从而有效地节省了处理能力和时间。

**删除 SASS 缓存文件夹:**可以删除 SASS 缓存文件夹，因为它基本上是缓存文件。它将在下一次编译时重新创建。但是，如果要重新编译某个模板的新文件，可能需要更长的时间，因为系统将不得不重新编译整个模板，而不是只重新编译已更改的部分。