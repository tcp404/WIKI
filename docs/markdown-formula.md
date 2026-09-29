# Markdown 公式语法

整理自[行无际《Markdown 公式语法》](https://www.cnblogs.com/bytesfly/p/markdown-formula.html#%E7%AC%A6%E5%8F%B7)的“符号”及后续章节。

原文版权声明：本文版权归作者和博客园共有。欢迎转载，但必须保留此段声明，且在文章页面明显位置给出原文连接！

行内公式用 `$...$`，独立成行的公式用 `$$...$$`。例如 $a^2+b^2=c^2$，对应语法是：

```markdown
勾股定理：$a^2+b^2=c^2$。

$$
a^2+b^2=c^2
$$
```

下表的反斜杠命令要写在数学公式定界符内；例如 `\frac{a}{b}` 可写成 `$\frac{a}{b}$`。

## 符号

### 上下标、运算符

| 用途               | 显示效果                                                                     | 语法示例                                                                     |
| ------------------ | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| 上标               | $x^2$、$e^{365}$                                                             | `x^2`、`e^{365}`                                                             |
| 下标               | $x_0$、$a_{ij}$                                                              | `x_0`、`a_{ij}`                                                              |
| 分式               | $\frac{x}{y}$、$\frac{1}{x+1}$                                               | `\frac{x}{y}`、`\frac{1}{x+1}`                                               |
| 乘、除             | $\times$、$\div$                                                             | `\times`、`\div`                                                             |
| 加减、减加         | $\pm$、$\mp$                                                                 | `\pm`、`\mp`                                                                 |
| 求和、求积         | $\sum$、$\prod$                                                              | `\sum`、`\prod`                                                              |
| 带上下限的求和     | $\sum_{i=0}^{n}$、$\sum_{i=0}^{\infty}$                                      | `\sum_{i=0}^{n}`、`\sum_{i=0}^{\infty}`                                      |
| 偏微分、积分       | $\partial$、$\int$、$\displaystyle\int$                                      | `\partial`、`\int`、`\displaystyle\int`                                      |
| 不等于             | $\neq$                                                                       | `\neq`                                                                       |
| 大于等于、小于等于 | $\geq$、$\leq$                                                               | `\geq`、`\leq`                                                               |
| 约等于、不大于等于 | $\approx$、$\ngeq$                                                           | `\approx`、`\ngeq`                                                           |
| 点乘、星乘         | $a\cdot b$、$a\ast b$                                                        | `a\cdot b`、`a\ast b`                                                        |
| 向下、向上取整     | $\left\lfloor\frac{a}{b}\right\rfloor$、$\left\lceil\frac{a}{b}\right\rceil$ | `\left\lfloor\frac{a}{b}\right\rfloor`、`\left\lceil\frac{a}{b}\right\rceil` |

上下标超过一个字符时，用花括号括起来，例如 $x_{i+1}^{n+1}$ 对应 `$x_{i+1}^{n+1}$`。

### 括号

| 用途     | 显示效果                                           | 语法示例                                                  |
| -------- | -------------------------------------------------- | --------------------------------------------------------- |
| 圆括号   | $\left(\frac{a}{b}\right)$                         | `\left(\frac{a}{b}\right)`                                |
| 方括号   | $\left[\frac{a}{b}\right]$                         | `\left[\frac{a}{b}\right]`                                |
| 花括号   | $\left\{\frac{a}{b}\right\}$、$\lbrace$、$\rbrace$ | `\left\{\frac{a}{b}\right\}`；也可用 `\lbrace`、`\rbrace` |
| 角括号   | $\left\langle\frac{a}{b}\right\rangle$             | `\left\langle\frac{a}{b}\right\rangle`                    |
| 混合括号 | $\left[a,b\right)$                                 | `\left[a,b\right)`                                        |

`\left` 与 `\right` 会随内容调整括号大小。只显示一侧时，另一侧用不可见定界符 `\left.` 或 `\right.` 补齐。

### 三角函数、指数、对数

| 用途       | 显示效果                        | 语法示例                        |
| ---------- | ------------------------------- | ------------------------------- |
| 正弦、余弦 | $\sin(x)$、$\cos(x)$            | `\sin(x)`、`\cos(x)`            |
| 正切、余切 | $\tan(x)$、$\cot(x)$            | `\tan(x)`、`\cot(x)`            |
| 指数       | $e^x$、$\exp(x)$                | `e^x`、`\exp(x)`                |
| 对数       | $\log_2 10$、$\lg 100$、$\ln 2$ | `\log_2 10`、`\lg 100`、`\ln 2` |

### 数学符号

| 用途                         | 显示效果                                                                 | 语法示例                                                                 |
| ---------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| 无穷                         | $\infty$                                                                 | `\infty`                                                                 |
| 向量                         | $\vec{a}$                                                                | `\vec{a}`                                                                |
| 一阶、二阶时间导数           | $\dot{x}$、$\ddot{x}$                                                    | `\dot{x}`、`\ddot{x}`                                                    |
| 上划线、帽号                 | $\bar{a}$、$\hat{a}$                                                     | `\bar{a}`、`\hat{a}`                                                     |
| 特殊虚数单位                 | $\imath$、$\jmath$                                                       | `\imath`、`\jmath`                                                       |
| 水平、居中、竖直、对角省略号 | $\ldots$、$\cdots$、$\vdots$、$\ddots$                                   | `\ldots`、`\cdots`、`\vdots`、`\ddots`                                   |
| 斜线、反斜线                 | $/$、$\backslash$                                                        | `/`、`\backslash`                                                        |
| 角度、撇号                   | $\angle$、$\prime$                                                       | `\angle`、`\prime`                                                       |
| 向右、向左箭头               | $\rightarrow$、$\leftarrow$                                              | `\rightarrow`、`\leftarrow`                                              |
| 向上、向下箭头               | $\uparrow$、$\downarrow$                                                 | `\uparrow`、`\downarrow`                                                 |
| 双线向右、向左箭头           | $\Rightarrow$、$\Leftarrow$                                              | `\Rightarrow`、`\Leftarrow`                                              |
| 向上、向下双线箭头           | $\Uparrow$、$\Downarrow$                                                 | `\Uparrow`、`\Downarrow`                                                 |
| 长箭头                       | $\longrightarrow$、$\longleftarrow$、$\Longrightarrow$、$\Longleftarrow$ | `\longrightarrow`、`\longleftarrow`、`\Longrightarrow`、`\Longleftarrow` |
| 梯度                         | $\nabla$                                                                 | `\nabla`                                                                 |
| 因为、所以                   | $\because$、$\therefore$                                                 | `\because`、`\therefore`                                                 |
| 整除或条件分隔               | $\mid$                                                                   | `\mid`                                                                   |
| 任意、存在                   | $\forall$、$\exists$                                                     | `\forall`、`\exists`                                                     |
| 相似、全等                   | $\backsim$、$\cong$                                                      | `\backsim`、`\cong`                                                      |
| 环路积分                     | $\oint$                                                                  | `\oint`                                                                  |
| 蕴含、等价、被蕴含           | $\implies$、$\iff$、$\impliedby$                                         | `\implies`、`\iff`、`\impliedby`                                         |

### 连线符号

| 用途                         | 显示效果                                                                           | 语法示例                                                                           |
| ---------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| 上方左箭头、右箭头、双向箭头 | $\overleftarrow{a+b+c}$、$\overrightarrow{a+b+c}$、$\overleftrightarrow{a+b+c}$    | `\overleftarrow{a+b+c}`、`\overrightarrow{a+b+c}`、`\overleftrightarrow{a+b+c}`    |
| 下方左箭头、右箭头、双向箭头 | $\underleftarrow{a+b+c}$、$\underrightarrow{a+b+c}$、$\underleftrightarrow{a+b+c}$ | `\underleftarrow{a+b+c}`、`\underrightarrow{a+b+c}`、`\underleftrightarrow{a+b+c}` |
| 上划线、下划线               | $\overline{a+b+c}$、$\underline{a+b+c}$                                            | `\overline{a+b+c}`、`\underline{a+b+c}`                                            |
| 上方、下方大括号             | $\overbrace{a+b+c}^{n}$、$\underbrace{a+b+c}_{n}$                                  | `\overbrace{a+b+c}^{n}`、`\underbrace{a+b+c}_{n}`                                  |
| 嵌套括号                     | $\overbrace{a+\underbrace{b+c}_{1}}^{2}$                                           | `\overbrace{a+\underbrace{b+c}_{1}}^{2}`                                           |
| 标注重复项                   | $\underbrace{a\cdot a\cdots a}_{n\text{ 次}}$                                      | `\underbrace{a\cdot a\cdots a}_{n\text{ 次}}`                                      |

### 高级运算符

| 用途               | 显示效果                                                             | 语法示例                                                             |
| ------------------ | -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| 平均值的上划线     | $\overline{xyz}$                                                     | `\overline{xyz}`                                                     |
| 平方根、$n$ 次方根 | $\sqrt{xy}$、$\sqrt[n]{x}$                                           | `\sqrt{xy}`、`\sqrt[n]{x}`                                           |
| 极限               | $\lim_{x\to\infty}f(x)$                                              | `\lim_{x\to\infty}f(x)`                                              |
| 求和               | $\sum_{i=1}^{n}i$                                                    | `\sum_{i=1}^{n}i`                                                    |
| 定积分             | $\int_0^{\infty}f(x)\,dx$                                            | `\int_0^{\infty}f(x)\,dx`                                            |
| 一阶、二阶偏导     | $\frac{\partial f}{\partial x}$、$\frac{\partial^2 f}{\partial x^2}$ | `\frac{\partial f}{\partial x}`、`\frac{\partial^2 f}{\partial x^2}` |

在行内公式中，`\displaystyle` 可让求和、积分等运算符显示为独立公式的大小，例如 $\displaystyle\sum_{i=1}^{n}i$ 对应 `$\displaystyle\sum_{i=1}^{n}i$`。

### 集合运算

| 用途                   | 显示效果                                       | 语法示例                                       |
| ---------------------- | ---------------------------------------------- | ---------------------------------------------- |
| 属于、不属于           | $x\in A$、$x\notin A$                          | `x\in A`、`x\notin A`                          |
| 子集、超集             | $A\subset B$、$B\supset A$                     | `A\subset B`、`B\supset A`                     |
| 子集或相等、超集或相等 | $A\subseteq B$、$B\supseteq A$                 | `A\subseteq B`、`B\supseteq A`                 |
| 严格真子集             | $A\subsetneq B$                                | `A\subsetneq B`                                |
| 并集、交集、差集       | $A\cup B$、$A\cap B$、$A\setminus B$           | `A\cup B`、`A\cap B`、`A\setminus B`           |
| 圈点、圈乘、圈加       | $A\bigodot B$、$A\bigotimes B$、$A\bigoplus B$ | `A\bigodot B`、`A\bigotimes B`、`A\bigoplus B` |
| 实数、整数、自然数集合 | $\mathbb{R}$、$\mathbb{Z}$、$\mathbb{N}$       | `\mathbb{R}`、`\mathbb{Z}`、`\mathbb{N}`       |

### 希腊字母

大写希腊字母中，与拉丁字母同形的可直接输入拉丁字母。

| 名称     | 显示效果               | 大写语法   | 小写语法   |
| -------- | ---------------------- | ---------- | ---------- |
| 阿尔法   | $A$、$\alpha$          | `A`        | `\alpha`   |
| 贝塔     | $B$、$\beta$           | `B`        | `\beta`    |
| 伽马     | $\Gamma$、$\gamma$     | `\Gamma`   | `\gamma`   |
| 德尔塔   | $\Delta$、$\delta$     | `\Delta`   | `\delta`   |
| 伊普西龙 | $E$、$\epsilon$        | `E`        | `\epsilon` |
| 泽塔     | $Z$、$\zeta$           | `Z`        | `\zeta`    |
| 伊塔     | $H$、$\eta$            | `H`        | `\eta`     |
| 西塔     | $\Theta$、$\theta$     | `\Theta`   | `\theta`   |
| 约塔     | $I$、$\iota$           | `I`        | `\iota`    |
| 卡帕     | $K$、$\kappa$          | `K`        | `\kappa`   |
| 兰布达   | $\Lambda$、$\lambda$   | `\Lambda`  | `\lambda`  |
| 缪       | $M$、$\mu$             | `M`        | `\mu`      |
| 纽       | $N$、$\nu$             | `N`        | `\nu`      |
| 克西     | $\Xi$、$\xi$           | `\Xi`      | `\xi`      |
| 奥密克戎 | $O$、$o$               | `O`        | `o`        |
| 派       | $\Pi$、$\pi$           | `\Pi`      | `\pi`      |
| 柔       | $P$、$\rho$            | `P`        | `\rho`     |
| 西格马   | $\Sigma$、$\sigma$     | `\Sigma`   | `\sigma`   |
| 陶       | $T$、$\tau$            | `T`        | `\tau`     |
| 宇普西龙 | $\Upsilon$、$\upsilon$ | `\Upsilon` | `\upsilon` |
| 斐       | $\Phi$、$\phi$         | `\Phi`     | `\phi`     |
| 希       | $X$、$\chi$            | `X`        | `\chi`     |
| 普西     | $\Psi$、$\psi$         | `\Psi`     | `\psi`     |
| 欧米伽   | $\Omega$、$\omega$     | `\Omega`   | `\omega`   |

常见变体还有 `\varepsilon`、`\vartheta`、`\varpi`、`\varrho`、`\varsigma` 和 `\varphi`。

### 字体转换

用字体命令包住需要转换的内容，例如 $\mathbf{ABC}$ 对应 `$\mathbf{ABC}$`。下表采用较通用的命令写法。

| 字体     | 显示效果              | 语法示例              |
| -------- | --------------------- | --------------------- |
| 正体     | $\mathrm{D}$          | `\mathrm{D}`          |
| 花体     | $\mathcal{D}$         | `\mathcal{D}`         |
| 意大利体 | $\mathit{D}$          | `\mathit{D}`          |
| 黑板粗体 | $\mathbb{D}$          | `\mathbb{D}`          |
| 粗体     | $\mathbf{D}$          | `\mathbf{D}`          |
| 无衬线体 | $\mathsf{D}$          | `\mathsf{D}`          |
| 手写体   | $\mathscr{D}$         | `\mathscr{D}`         |
| 打字机体 | $\mathtt{D}$          | `\mathtt{D}`          |
| 哥特体   | $\mathfrak{D}$        | `\mathfrak{D}`        |
| 粗体符号 | $\boldsymbol{\alpha}$ | `\boldsymbol{\alpha}` |

原文还使用 `\rm`、`\cal`、`\it`、`\Bbb`、`\bf`、`\mit`、`\sf`、`\scr`、`\tt`、`\frak` 等简写；不同渲染器对这些旧写法的支持可能不同。

## 公式

### 基本函数公式

行内公式：$\Gamma(z)=\int_0^\infty t^{z-1}e^{-t}\,dt$，语法为 `$\Gamma(z)=\int_0^\infty t^{z-1}e^{-t}\,dt$`。

独立公式：

显示效果：

$$
\Gamma(z)=\int_0^\infty t^{z-1}e^{-t}\,dt
$$

语法：

```markdown
$$
\Gamma(z)=\int_0^\infty t^{z-1}e^{-t}\,dt
$$
```

更多行内示例：

显示效果：

$y_k=\varphi(u_k+v_k)$

$y(x)=x^3+2x^2+x+1$

$x^y=(1+\mathrm{e}^x)^{-2xy}$

$\displaystyle f(n)=\sum_{i=1}^{n}i$

语法：

```markdown
$y_k=\varphi(u_k+v_k)$
$y(x)=x^3+2x^2+x+1$
$x^y=(1+\mathrm{e}^x)^{-2xy}$
$\displaystyle f(n)=\sum_{i=1}^{n}i$
```

### 分段函数

`cases` 中的 `&` 分隔公式和条件，`\\` 换行。

显示效果：

$$
y=\begin{cases}
2x+1, & x\leq 0 \\
x, & x>0
\end{cases}
$$

语法：

```markdown
$$
y=\begin{cases}
2x+1, & x\leq 0 \\
x, & x>0
\end{cases}
$$
```

方程组也可用 `array` 排列：

显示效果：

$$
\left\{
\begin{array}{c}
a_1x+b_1y+c_1z=d_1 \\
a_2x+b_2y+c_2z=d_2 \\
a_3x+b_3y+c_3z=d_3
\end{array}
\right.
$$

语法：

```markdown
$$
\left\{
\begin{array}{c}
a_1x+b_1y+c_1z=d_1 \\
a_2x+b_2y+c_2z=d_2 \\
a_3x+b_3y+c_3z=d_3
\end{array}
\right.
$$
```

### 积分

显示效果：

$$
\int_{a}^{b}f(x)\,dx
$$

$$
\iint_D f(x,y)\,dx\,dy
$$

$$
\iiint_V f(x,y,z)\,dx\,dy\,dz
$$

语法：

```markdown
$$
\int_{a}^{b}f(x)\,dx
$$

$$
\iint_D f(x,y)\,dx\,dy
$$

$$
\iiint_V f(x,y,z)\,dx\,dy\,dz
$$
```

### 微分和偏微分

显示效果：

$$
\frac{dy}{dx}+P(x)y=Q(x)
$$

$$
\left.\frac{dy}{dx}\right|_{x=0}=1
$$

$$
y''+py'+qy=f(x)
$$

$$
\frac{d^2y}{dx^2}+p\frac{dy}{dx}+qy=f(x)
$$

$$
\frac{\partial u}{\partial t}
=h^2\left(
\frac{\partial^2u}{\partial x^2}
+\frac{\partial^2u}{\partial y^2}
+\frac{\partial^2u}{\partial z^2}
\right)
$$

语法：

```markdown
$$
\frac{dy}{dx}+P(x)y=Q(x)
$$

$$
\left.\frac{dy}{dx}\right|_{x=0}=1
$$

$$
y''+py'+qy=f(x)
$$

$$
\frac{d^2y}{dx^2}+p\frac{dy}{dx}+qy=f(x)
$$

$$
\frac{\partial u}{\partial t}
=h^2\left(
\frac{\partial^2u}{\partial x^2}
+\frac{\partial^2u}{\partial y^2}
+\frac{\partial^2u}{\partial z^2}
\right)
$$
```

### 矩阵和行列式

矩阵环境以 `\begin{matrix}` 开始、`\end{matrix}` 结束；`&` 分隔列，`\\` 换行。替换环境名称可改变外框：

| 环境      | 显示效果                               | 外框                 |
| --------- | -------------------------------------- | -------------------- |
| `matrix`  | $\begin{matrix}1&2\\3&4\end{matrix}$   | 无                   |
| `pmatrix` | $\begin{pmatrix}1&2\\3&4\end{pmatrix}$ | 圆括号               |
| `bmatrix` | $\begin{bmatrix}1&2\\3&4\end{bmatrix}$ | 方括号               |
| `Bmatrix` | $\begin{Bmatrix}1&2\\3&4\end{Bmatrix}$ | 花括号               |
| `vmatrix` | $\begin{vmatrix}1&2\\3&4\end{vmatrix}$ | 单竖线，常用于行列式 |
| `Vmatrix` | $\begin{Vmatrix}1&2\\3&4\end{Vmatrix}$ | 双竖线               |

显示效果：

$$
A=\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
$$

$$
I=\begin{bmatrix}
1&0&0 \\
0&1&0 \\
0&0&1
\end{bmatrix}
$$

$$
A=\begin{bmatrix}
a_{11}&a_{12}&\cdots&a_{1n} \\
a_{21}&a_{22}&\cdots&a_{2n} \\
\vdots&\vdots&\ddots&\vdots \\
a_{m1}&a_{m2}&\cdots&a_{mn}
\end{bmatrix}
$$

$$
D=\begin{vmatrix}
a_{11}&a_{12} \\
a_{21}&a_{22}
\end{vmatrix}
$$

语法：

```markdown
$$
A=\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
$$

$$
I=\begin{bmatrix}
1&0&0 \\
0&1&0 \\
0&0&1
\end{bmatrix}
$$

$$
A=\begin{bmatrix}
a_{11}&a_{12}&\cdots&a_{1n} \\
a_{21}&a_{22}&\cdots&a_{2n} \\
\vdots&\vdots&\ddots&\vdots \\
a_{m1}&a_{m2}&\cdots&a_{mn}
\end{bmatrix}
$$

$$
D=\begin{vmatrix}
a_{11}&a_{12} \\
a_{21}&a_{22}
\end{vmatrix}
$$
```

带分隔线的增广矩阵用 `array`：

显示效果：

$$
\left[
\begin{array}{cc|c}
1&2&3 \\
4&5&6
\end{array}
\right]
$$

语法：

```markdown
$$
\left[
\begin{array}{cc|c}
1&2&3 \\
4&5&6
\end{array}
\right]
$$
```

## 案例

### 上下标与自动伸缩的括号

显示效果：

$$
x^{y^z}=(1+\mathrm{e}^x)^{-2xy^w}
$$

$$
f(x,y,z)=3y^2z\left(3+\frac{7x+5}{1+y^2}\right)
$$

语法：

```markdown
$$
x^{y^z}=(1+\mathrm{e}^x)^{-2xy^w}
$$

$$
f(x,y,z)=3y^2z\left(3+\frac{7x+5}{1+y^2}\right)
$$
```

使用 `\left.` 或 `\right.` 可隐藏配对的一侧，例如在导数旁标出取值点：

显示效果：

$$
\left.\frac{du}{dx}\right|_{x=0}
$$

语法：

```markdown
$$
\left.\frac{du}{dx}\right|_{x=0}
$$
```

### 公式编号与注释

`\tag{...}` 可以给独立公式添加编号；`\text{...}` 用来插入普通文字。

显示效果：

$$
E=mc^2\tag{1}
$$

$$
f(n)=\begin{cases}
n/2, & \text{当 }n\text{ 为偶数} \\
3n+1, & \text{当 }n\text{ 为奇数}
\end{cases}
$$

语法：

```markdown
$$
E=mc^2\tag{1}
$$

$$
f(n)=\begin{cases}
n/2, & \text{当 }n\text{ 为偶数} \\
3n+1, & \text{当 }n\text{ 为奇数}
\end{cases}
$$
```

### 对齐的推导

在 `align` 中用 `&` 标出对齐位置，用 `\\` 换行。

显示效果：

$$
\begin{align}
(a+b)^2
&=(a+b)(a+b) \\
&=a^2+2ab+b^2
\end{align}
$$

语法：

```markdown
$$
\begin{align}
(a+b)^2
&=(a+b)(a+b) \\
&=a^2+2ab+b^2
\end{align}
$$
```

逐行写出推导理由时，可以增加一列 `\text{...}`：

显示效果：

$$
\begin{align}
v+w &= 0 & \text{已知} \\
-w &= -w+0 & \text{加法单位元} \\
-w+0 &= -w+(v+w) & \text{代入}
\end{align}
$$

语法：

```markdown
$$
\begin{align}
v+w &= 0 & \text{已知} \\
-w &= -w+0 & \text{加法单位元} \\
-w+0 &= -w+(v+w) & \text{代入}
\end{align}
$$
```

用 `array` 的 `l` 列格式，也可以把说明文字左对齐：

显示效果：

$$
\left.
\begin{array}{ll}
\text{若 }n\text{ 为偶数：} & n/2 \\
\text{若 }n\text{ 为奇数：} & 3n+1
\end{array}
\right\}=f(n)
$$

语法：

```markdown
$$
\left.
\begin{array}{ll}
\text{若 }n\text{ 为偶数：} & n/2 \\
\text{若 }n\text{ 为奇数：} & 3n+1
\end{array}
\right\}=f(n)
$$
```

### 连分式

用 `\cfrac` 使嵌套分数保持较大的字号：

显示效果：

$$
x=a_0+\cfrac{1}{a_1+\cfrac{1}{a_2+\cfrac{1}{a_3+\cdots}}}
$$

语法：

```markdown
$$
x=a_0+\cfrac{1}{a_1+\cfrac{1}{a_2+\cfrac{1}{a_3+\cdots}}}
$$
```

### 公式中的表格

`array` 的列格式中，`l`、`c`、`r` 分别表示左、中、右对齐；`|` 是竖线，`\hline` 是横线。

显示效果：

$$
\begin{array}{c|lcr}
n & \text{左对齐} & \text{居中} & \text{右对齐} \\
\hline
1 & 0.24 & 1 & 125 \\
2 & -1 & 189 & -8 \\
3 & -20 & 2000 & 1+10i
\end{array}
$$

语法：

```markdown
$$
\begin{array}{c|lcr}
n & \text{左对齐} & \text{居中} & \text{右对齐} \\
\hline
1 & 0.24 & 1 & 125 \\
2 & -1 & 189 & -8 \\
3 & -20 & 2000 & 1+10i
\end{array}
$$
```
