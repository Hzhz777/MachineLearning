# LaTeX 数学符号速查表

适合机器学习学习笔记，包含公式源码与显示效果。显示效果需要支持 LaTeX 数学公式的 Markdown 阅读器。

## 在 Jupyter 中写公式

在 Jupyter 的 Markdown 单元格里使用以下写法：

```markdown
行内公式：$y = wx + b$

单独一行的公式：
$$
y = wx + b
$$
```

写完按 `Shift + Enter` 显示公式。使用英文的 `$` 和反斜杠 `\`。

## 基础写法

| 含义 | LaTeX 写法 | 显示效果 |
|---|---|---|
| 下标 | `x_i` | $x_i$ |
| 多字符下标 | `x_{train}` | $x_{train}$ |
| 上标或次方 | `x^2` | $x^2$ |
| 多字符上标 | `x^{10}` | $x^{10}$ |
| 样本编号 | `x^{(i)}` | $x^{(i)}$ |
| 分数 | `\frac{a}{b}` | $\frac{a}{b}$ |
| 平方根 | `\sqrt{x}` | $\sqrt{x}$ |
| n 次方根 | `\sqrt[n]{x}` | $\sqrt[n]{x}$ |
| 绝对值 | `\lvert x \rvert` | $\lvert x \rvert$ |
| 范数 | `\lVert x \rVert_2` | $\lVert x \rVert_2$ |
| 预测值或帽子符号 | `\hat{y}` | $\hat{y}$ |
| 平均值或上横线 | `\bar{x}` | $\bar{x}$ |
| 向量箭头 | `\vec{x}` | $\vec{x}$ |
| 粗体向量 | `\mathbf{x}` | $\mathbf{x}$ |

## 运算与比较

| 含义 | LaTeX 写法 | 显示效果 |
|---|---|---|
| 乘号 | `\times` | $\times$ |
| 点乘号 | `\cdot` | $\cdot$ |
| 除号 | `\div` | $\div$ |
| 正负号 | `\pm` | $\pm$ |
| 不等于 | `\neq` | $\neq$ |
| 小于等于 | `\leq` | $\leq$ |
| 大于等于 | `\geq` | $\geq$ |
| 约等于 | `\approx` | $\approx$ |
| 正比于 | `\propto` | $\propto$ |
| 无穷大 | `\infty` | $\infty$ |
| 属于 | `\in` | $\in$ |
| 实数集合 | `\mathbb{R}` | $\mathbb{R}$ |
| n 维实数空间 | `\mathbb{R}^n` | $\mathbb{R}^n$ |
| 右箭头 | `\rightarrow` | $\rightarrow$ |
| 趋于 | `\to` | $\to$ |
| 推出 | `\Rightarrow` | $\Rightarrow$ |

## 常见希腊字母

| 含义 | LaTeX 写法 | 显示效果 |
|---|---|---|
| alpha | `\alpha` | $\alpha$ |
| beta | `\beta` | $\beta$ |
| gamma | `\gamma` | $\gamma$ |
| delta | `\delta` | $\delta$ |
| 大写 Delta | `\Delta` | $\Delta$ |
| epsilon | `\epsilon` | $\epsilon$ |
| theta | `\theta` | $\theta$ |
| lambda | `\lambda` | $\lambda$ |
| mu | `\mu` | $\mu$ |
| sigma | `\sigma` | $\sigma$ |
| pi | `\pi` | $\pi$ |

## 求和、导数与梯度

| 含义 | LaTeX 写法 | 显示效果 |
|---|---|---|
| 求和 | `\sum_{i=1}^{m} x_i` | $\sum_{i=1}^{m} x_i$ |
| 连乘 | `\prod_{i=1}^{m} x_i` | $\prod_{i=1}^{m} x_i$ |
| 一阶导数 | `f'(x)` | $f'(x)$ |
| 导数的分式写法 | `\frac{d f}{d x}` | $\frac{d f}{d x}$ |
| 偏导符号 | `\partial` | $\partial$ |
| 对 w 的偏导 | `\frac{\partial J}{\partial w}` | $\frac{\partial J}{\partial w}$ |
| 梯度 | `\nabla J` | $\nabla J$ |
| 极限 | `\lim_{x \to 0} f(x)` | $\lim_{x \to 0} f(x)$ |
| 最小值 | `\min_{w,b} J(w,b)` | $\min_{w,b} J(w,b)$ |
| 自然对数 | `\ln x` | $\ln x$ |
| 指数 | `e^x` | $e^x$ |

## 括号、文字和多行公式

括号自动适应里面的内容大小：

```latex
\left( \frac{a}{b} \right)
```

$$
\left( \frac{a}{b} \right)
$$

公式里插入普通文字：

```latex
x_{\text{train}}
```

$$
x_{\text{train}}
$$

多行公式中，`\\` 表示换行，`&` 标记对齐位置：

```latex
\begin{aligned}
a &= b + c \\
d &= e + f
\end{aligned}
```

$$
\begin{aligned}
a &= b + c \\
d &= e + f
\end{aligned}
$$

矩阵中，`&` 分隔列，`\\` 分隔行：

```latex
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
```

$$
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
$$

## 分组规则

`{...}` 是分组，不会显示出来。比如 `x^10` 只会把 `1` 放到上标位置，要写成 `x^{10}` 才能让整个 `10` 成为上标。

