---
html:
  embed_local_images: false
  embed_svg: true
  offline: false
  toc: true
toc:
  depth_from: 1
  depth_to: 6
  ordered: true
print_background: false
---

# 函数

## 函数的变换

对于函数$$y = f(x)$$



![png](https://s1.ax1x.com/2020/10/16/0b4kX6.png)


其上任意一点$$\begin{array}{l}  
  (x_0,f(x_0))\\  
  y_0 = f(x_0)\\
\end{array}$$

首先对其做平移变换，将函数向左平移$\pi\over2$个单位得到$$(x_0-\frac{\pi}{2},f(x_0))$$


![png](https://s1.ax1x.com/2020/10/16/0b4uhd.png)


再对其进行伸缩变换，使此刻所有横坐标变为原来的2倍得到$$(2(x_0-\frac{\pi}{2}),f(x_0))$$



![png](https://s1.ax1x.com/2020/10/16/0b4gN4.png)


再在竖直方向进行拉伸两倍得到$$(2(x_0-\frac{\pi}{2}),2f(x_0))$$



![png](https://s1.ax1x.com/2020/10/16/0b4cEF.png)


最后得到关系式$$\begin{array}{l}  
  x'=2x_0-\pi \\  
  y'=2y_0 \\
\end{array} $$
其中$y_0 = f(x_0)$

变换可得$$\begin{array}{l} 
  x_0=\frac{1}{2}x'+\frac{\pi}{2}\\
  y_0 = \frac{1}{2}y'
\end{array} $$

带入可得$$\frac{1}{2}y'=f(\frac{1}{2}x'+\frac{\pi}{2})$$

容易知道对于任意的$$\begin{array}{l}
(x',y')\\
y=2f(\frac{1}{2}x+\frac{\pi}{2})
\end{array}$$



![png](https://s1.ax1x.com/2020/10/16/0b4yHU.png)


同理，对于$$y=f(x)$$

先把横坐标拉伸2倍$$(2x_0,y_0)$$


![png](https://s1.ax1x.com/2020/10/16/0b4OCd.png)


再右移3个单位$$(2x_0+3,y_0)$$


![png](https://s1.ax1x.com/2020/10/16/0b4X8A.png)


再竖着拉伸$\frac{1}{3}$倍$$(2x_0+3,\frac{1}{3}y_0)$$


![png](https://s1.ax1x.com/2020/10/16/0b4jgI.png)


有对应关系$$\begin{array}{l}
x'=2x_0+3\\
y'=\frac{1}{3}y_0
\end{array}$$

代入有$$y' = \frac{1}{3}f(\frac{1}{2}(x'-3))$$



![png](https://s1.ax1x.com/2020/10/16/0b4vvt.png)


## 实例详解

把$$y = f(\omega x+\phi)$$向左平移m个单位

对于点$$(x_0,y_0)$$有映射$$f:\omega x_0+\phi \longrightarrow y_0 $$

平移后的点为$$(x_0-m,y_0)$$

记$x_0-m=x_1$则有映射$$f:\omega(x_1+m)+\phi\longrightarrow y_0$$

即对于变换后的点而言任意给出的x与y有关系式$$y=f(\omega (x+m)+\phi)$$

直接有**推论**$$y=f(\omega x+\phi)=f(\omega (x+\frac{\phi}{\omega}))$$可以由$$y=f(\omega x)$$向左平移$\frac{\phi}{\omega}$个单位得到

同理，把$$y = f(\omega x+\phi)$$在水平方向拉伸k倍

拉伸后的点为$$(kx_0,y_0)$$

记$x_2 = kx_0$有$$f:\omega\frac{x_2}{k}+\phi\longrightarrow y_0$$

平移后的函数即为$$y=f(\omega\frac{x_2}{k}+\phi)$$

### 推论

在水平方向的伸缩不改变$\phi$

水平方向的平移作用在$\omega$的括号里

如何快速$$y=f(\omega_1 x+\phi_1)\longrightarrow y= f(\omega_2 x+\phi_2)$$

根据推论首先改$\omega$不改变$\phi$

即在水平方向伸缩$\frac{\omega_1}{\omega_2}$倍得到$$\begin{array}{l}\omega_1 x_0=\omega_2 x_1\\x_1=\frac{\omega_1}{\omega_2}x_0\end{array}$$

然后再水平平移，我不写了，你懂得

## 奇怪的题

锐角三角形ABC中，欲证$$sin A+sin B+sin C>cos A+cos B+cos C$$

注意到$$A+B>\frac{\pi}{2}$$


![png](https://s1.ax1x.com/2020/10/16/0b4q4H.png)


注意到$$\frac{\pi}{4}-A<B-\frac{\pi}{4}$$

所以有$$sinA>cosB$$得证

# 易错点

## 注意平凡情况

比如斜率为0啊，二次函数首项系数为0啊啥的，这一写，不就有分了？先写上再说

导数切线题注意看好，是 ***在*** 某点的切线，还是 ***过*** 某点的切线

概率题，把事件写上，要不然扣分！

## 咱们来看看一个简单的矩阵

$$ \begin{bmatrix}  
  a_{11}& a_{12}& \cdots  & a_{1n} \\  
  a_{21}& a_{22}& \cdots  & a_{2n} \\  
  \vdots & \vdots & \ddots & \vdots \\  
  a_{m1}& a_{m2}& \cdots  & a_{mn}  
\end{bmatrix}  $$

条件告诉你$$a_{ik}\ne a_{jk}$$说的是啥意思呢

说的是同一列中的第i个和第j个不等！

## 有关向量的角度

注意到向量的角度从0取到$\pi$，其中，0不是锐角，$\pi$不是钝角

# 圆锥曲线

## 二次曲线系

简单回顾

对于任意二次曲线$$\begin{array}{l}A_1x^2+B_1y^2+C_1xy+D_1x+E_1y+F_1=0\\A_2x^2+B_2y^2+C_2xy+D_2x+E_2y+F_2=0\end{array}$$

过它们交点的二次曲线可以写成$$\mu(A_1x^2+B_1y^2+C_1xy+D_1x+E_1y+F_1)+\lambda(A_2x^2+B_2y^2+C_2xy+D_2x+E_2y+F_2)=0$$

这时候，只要配配系数就可以解决问题了

比如圆的方程必没有xy项，且$x^2$和$y^2$系数相等

### 实例详解

椭圆$$Ax^2+By^2+F=0$$

椭圆外一点E在定直线x=C上运动，与左顶点A与右顶点B连直线交椭圆于四个点ACBD

证明AB与CD交点为定点

只需设出$l_{EA}$和$l_{EB}$的方程并乘在一块再与椭圆方程构建二次曲线系

就可以得到一定过ABCD四个点的二次曲线

随后，把$l_{AB}$和$l_{CD}$的直线根据CD过定点设出来，调参数即可

## 中点弦

中点弦是指，这有一个点，过这个点的直线与二次曲线恰好交于两点，这个点是中点，那么这条直线就能确定了

对于任意二次曲线$$Ax^2+By^2+Cxy+Dx+Ey+F=0$$

设$$(x_0,y_0)$$为那个中点

则有另外两个被分成两段的点$$(x_1,y_1),(2x_0-x_1,2y_0-y_1)$$

立刻有方程$$\begin{array}{l}
Ax_1^2+By_1^2+Cx_1y_1+Dx_1+Ey_1+F=0 \qquad(1)\\
A(2x_0-x_1)^2+B(2y_0-y_1)^2+C(2x_0-x_1)(2y_0-y_1)+D(2x_0-x_1)+E(2y_0-y_1)+F=0 \qquad(2)
\end{array}$$

(2)-(1)得到$$A(4x_0^2-4x_0x_1)+B(4y_0^2-4y_0y_1)+C(4x_0y_0-2(x_0y_1+y_0x_1))+D(2x_0-2x_1)+E(2y_0-2y_1)=0$$

化简得到$$(2Ax_0+Cy_0+D)(x_1-x_0)+(2By_0+Cx_0+E)(y_1-y_0)=0$$

看得到$$(2Ax_0+Cy_0+D,2By_0+Cx_0+E)$$是该直线的法向量

所以中点弦即为$$(2Ax_0+Cy_0+D)(x-x_0)+(2By_0+Cx_0+E)(y-y_0)=0$$

或者这个形式$$(2Ax_0+Cy_0+D)x+(2By_0+Cx_0+E)y=(2Ax_0+Cy_0+D)x_0+(2By_0+Cx_0+E)y_0$$

注意到$(x_0,y_0)$关于该曲线的极线为$$Ax_0x+By_0y+C\frac{x_0y+y_0x}{2}+D\frac{x_0+x}{2}+E\frac{y_0+y}{2}+F=0$$

或者换一种写法$$(2Ax_0+Cy_0+D)x+(2By_0+Cx_0+E)y=-2F$$形式相近，方便记忆

### 结论

求中点弦只要把这个点的极线写出来，左边只放x和y，在右边放x和y对应前面的系数和$x_0,y_0$

举例，椭圆$Ax^2+By^2+F=0$的中点弦是$$Ax_0x+By_0y=Ax_0^2+By_0^2$$

![1.jpg](https://s1.ax1x.com/2020/10/16/0b5DGd.jpg)

# 小技巧

## 代数

见到形如$$xy+\frac{1}{x}+\frac{1}{y}=1$$的式子该怎么处理呢？

①可以两边乘以xy然后当作x的二次函数来解

②可以利用$$(a+1)(b+1)=ab+a+b+1$$这个结论

③换元$$\left\{\begin{matrix} 
  xy=a \\  
  \frac{1}{x}=b \\
    \frac{1}{y}=c 
\end{matrix}\right. $$

有$$\left\{\begin{matrix} 
  a+b+c=1 \\  
  abc=1
\end{matrix}\right. $$

## 数论

对于偶数来说，可以表示为$2^n$以及$2^m\cdot c$其中$$c=2k+1\quad k\in\mathbb{N^+} $$

对于$$(i+j)(i-j)\quad (i,j\in \mathbb{N^+})$$

可以表示除了1，2之外的所有自然数

而对于$$(i+j)(i-j+1)\quad (i,j\in \mathbb{N^+})$$

来说，可以表示除了2的幂之外的所有偶数

给定一个不是2的幂的偶数，必然能写成$$2^m\cdot c \quad\text{where}\quad c=2k+1\quad k\in \mathbb{N^+}$$

则只需令$$\begin{array}{l}
i+j=2^m\\
i-j+1=c=2k+1
\end{array}$$

就能解出一组(i,j)
