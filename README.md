# 神经网络数学讲义

从单个神经元出发，介绍前馈神经网络的函数表示、ReLU 激活、映射复合与逼近理论。讲义以两页手写笔记为基础整理，补充符号约定、定理适用范围及参考文献，适合具备基础线性代数与数学分析知识的读者。

## 开始阅读

- **[在线阅读完整讲义](神经网络讲义.md)**：正文包含 LaTeX 公式、网络示意图和原始手写笔记。
- **[离线阅读版](神经网络讲义_离线阅读.html)**：下载此 HTML 文件后，用浏览器打开；图片和字体已内嵌。GitHub 文件页面可能显示源码，请下载后阅读。

## 内容

1. 什么是神经网络：参数化函数、表达能力与逼近能力。
2. 单个神经元：仿射映射、ReLU 与非线性的作用。
3. 网络的组合：单隐藏层、多隐藏层及层数计数。
4. 数学原理：万能逼近性、深度分离及两者的区别。
5. 原始手写笔记：两页原图供对照核验。

## 符号约定

隐藏层逐坐标使用 ReLU，输出层采用仿射映射；输入层不计入深度。单隐藏层网络包含两个仿射层。万能逼近性是存在性结论，不意味着固定宽度足够，也不保证训练算法能够找到对应参数。

## 文件结构

```text
.
├── README.md
├── 神经网络讲义.md
├── 神经网络讲义_离线阅读.html
└── 配图/
    ├── 神经元与ReLU.png / .svg
    ├── ReLU函数.png / .svg
    ├── 单隐藏层网络.png / .svg
    ├── 手写笔记-第1页.jpg
    └── 手写笔记-第2页.jpg
```

PNG 用于正文展示，SVG 保留为矢量版本。正文图片采用相对路径；下载整个仓库后，请保持目录结构不变。

## 编辑与勘误

以 `神经网络讲义.md` 为正文编辑源。行内公式使用 `$...$`，独立公式使用 `$$` 包围的块；GitHub 支持这些数学表达式，详见 [GitHub 数学公式文档](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)。

离线 HTML 是独立快照，修改 Markdown 或配图不会自动更新 HTML，修订后需同步重新导出。欢迎通过 Issue 或 Pull Request 提交勘误，请注明章节、原文和建议修改内容。

## 参考文献

正文给出了所用结论的范围和文献链接：

- Leshno、Lin、Pinkus 与 Schocken（1993）：[连续非多项式激活函数的万能逼近结果](https://pinkus.net.technion.ac.il/files/2021/02/neural.pdf)。
- Eldan 与 Shamir（2016）：[The Power of Depth for Feedforward Neural Networks](https://proceedings.mlr.press/v49/eldan16.html)，COLT，PMLR 49:907–940。

## 使用许可

本仓库暂未附加开源许可证。公开阅读不等同于授予任意转载、改编或再分发许可；如需复用，请先联系相应权利人。引用论文的权利归其相应权利人所有。
