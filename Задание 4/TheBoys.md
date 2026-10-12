# Вычисление ленточного определителя (трехдиагональной матрицы)

**Вариант 12**

```math
A = \begin{pmatrix}
7 & 6 & 0 & \dots & 0 & 0 \\
2 & 7 & 6 & \dots & 0 & 0 \\
0 & 2 & 7 & \dots & 0 & 0 \\
\vdots & \vdots & \vdots & \ddots & \vdots & \vdots \\
0 & 0 & 0 & \dots & 7 & 6 \\
0 & 0 & 0 & \dots & 2 & 7
\end{pmatrix}
```

Порядок матрицы $n = 9$

$$7X_{n-1} + 6(-2 \cdot X_{n-2})$$

$$\boxed{X_n = 7X_{n-1} - 12X_{n-2}} \quad \leftarrow X_3$$

$$X_1 = 7$$

$$X_2 = 7 \cdot 7 - 6 \cdot 2 = 37$$

## 1. Характеристическое уравнение

$$X_n \to \lambda^n$$

$$\lambda^n = 7 \cdot \lambda^{n-1} - 12\lambda^{n-2} \quad \Big| : \lambda^{n-2}$$

$$\lambda^2 = 7 \cdot \lambda - 12 = 0$$

$$\lambda^2 - 7\lambda + 12 = 0 \quad \leftarrow \text{квадратное уравнение}$$

$$D = (-7)^2 - 4 \cdot 1 \cdot 12$$

$$D = 49 - 4 \cdot 12 = 49 - 48 = 1 \qquad \boxed{D = b^2 - 4ac}$$

$$x_1 = \frac{7 + \sqrt{1}}{2 \cdot 1} = \frac{7 + 1}{2} = \frac{8}{2} = 4 \qquad \boxed{X_1 = \frac{-b + \sqrt{D}}{2a}}$$

$$x_2 = \frac{7 - \sqrt{1}}{2 \cdot 1} = \frac{7 - 1}{2} = \frac{6}{2} = 3 \qquad \boxed{X_2 = \frac{-b - \sqrt{D}}{2a}}$$

## 2. Общее решение

$$\boxed{X_n = A_1 \cdot 4^n + A_2 \cdot 3^n}$$

$$X_1 = A_1 \cdot 4^1 + A_2 \cdot 3^1 \qquad X_1 = 7$$

$$X_2 = A_1 \cdot 4^2 + A_2 \cdot 3^2 \qquad X_2 = 37$$

```math
\begin{cases}
7 = A_1 \cdot 4 + A_2 \cdot 3 \\
37 = A_1 \cdot 16 + A_2 \cdot 9
\end{cases}
```

Умножим первое уравнение на 3:

$$21 = A_1 \cdot 12 + A_2 \cdot 9$$

Вычтем полученное уравнение из второго уравнения системы:

$$37 - 21 = A_1 \cdot 16 - A_1 \cdot 12 + A_2 \cdot 9 - A_2 \cdot 9$$

$$16 = A_1 \cdot 4$$

$$A_1 = \frac{16}{4} = 4$$

Подставим $A_1 = 4$ в первое уравнение системы:

$$7 = 4 \cdot 4 + A_2 \cdot 3$$

$$7 = 16 + A_2 \cdot 3$$

$$A_2 \cdot 3 = 7 - 16 = -9$$

$$A_2 = \frac{-9}{3} = -3$$

Проверка (второе уравнение): $4 \cdot 16 + (-3) \cdot 9 = 64 - 27 = 37$ — верно.

$$A_1 = 4$$

$$A_2 = -3$$

## 3. Вычисление определителя для n = 9

$$\boxed{X_n = 4 \cdot 4^n + (-3) \cdot 3^n}$$

$$X_9 = 4 \cdot 4^9 + (-3) \cdot 3^9$$

$$X_9 = 4 \cdot 262144 + (-3) \cdot 19683$$

$$X_9 = 1048576 - 59049$$

$$X_9 = 989527$$
