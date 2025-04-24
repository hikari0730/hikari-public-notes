給定一階線性微分方程式 $\frac{dy}{dx}+P(x)y=Q(x)$，若存在 $\mu(x)$ 同乘等式兩側後，等式左側滿足 $\frac{d}{dx}(\mu(x)y)=\mu(x)\frac{dy}{dx}+\mu(x)P(x)y$

即 $\frac{d\mu(x)}{dx} = \mu(x)P(x)$時 ,則稱 $\mu(x)$為該微分方程式的積分因子。

---

## 積分因子的定義｜Definition of the Integrating Factor

給定一個一階線性微分方程式：  
**Given a first-order linear differential equation:**  
`dy/dx + P(x)y = Q(x)`

若存在某函數 $\mu(x)$ 同乘於等式兩側，使得左側滿足下列關係：  
**If there exists a function $\mu(x)$ such that, after multiplying both sides of the equation, the left-hand side satisfies:**  
`d/dx [μ(x)y] = μ(x) dy/dx + μ(x)P(x)y`

即  
**That is,**  
`dμ(x)/dx = μ(x)P(x)`

則稱 $\mu(x)$ 為該微分方程式的 **積分因子**。  
**Then $\mu(x)$ is called the _integrating factor_ of the differential equation.**

## 如何求得 $\mu(x)$?
給定 $\frac{d\mu(x)}{dx} = \mu(x)P(x)$,
移項後 
$\frac{\frac{d\mu(x)}{dx}}{\mu(x)} = P(x)$, 因為 $\frac{dln(x)}{dx}=\frac{1}{x}$以及根據連鎖律，原等式 $\frac{\frac{d\mu(x)}{dx}}{\mu(x)} = P(x)$可由 
$\frac{dln(\mu(x))}{dx}
=（\frac{dln(\mu(x))}{d\mu(x)}）\times(\frac{d\mu(x)}{dx})
= \frac{\frac{d\mu(x)}{dx}}{\mu(x)}
= P(x)$算式推導得出與 $ln(\mu(x))$的關係, 等式兩邊再同時積分， $\int\frac{dln(\mu(x))}{dx}dx
= \int P(x)dx$， 
$ln(\mu(x)) = \int P(x)dx$ ，
兩邊取指數,  
$\mu(x) = e^{\int P(x)dx}$，
即可求得積分因子 $\mu(x)$。

---

## 如何求得積分因子 $\mu(x)$？  
**How to find the integrating factor $\mu(x)$?**

給定一階線性微分方程的積分因子微分式：
Given: $\frac{d\mu(x)}{dx} = \mu(x)P(x)$

將等式改寫為變數分離形式：
Rewrite: $\frac{\frac{d\mu(x)}{dx}}{\mu(x)} = P(x)$

由 $\frac{d}{dx}[\ln(\mu(x))] = \frac{1}{\mu(x)}\cdot \frac{d\mu(x)}{dx}$（連鎖律）可得：

```text
d/dx [ln(μ(x))] 
= (d/dμ(x) [ln(μ(x))]) × (dμ(x)/dx)
= (1/μ(x)) × dμ(x)/dx
= P(x)
```

Since: $\frac{d}{dx}[\ln(\mu(x))] = \frac{1}{\mu(x)} \cdot \frac{d\mu(x)}{dx} = P(x)$

兩邊同時積分：

$\int \frac{d}{dx} \ln(\mu(x)) dx = \int P(x) dx$
$\ln(\mu(x)) = \int P(x) dx$

兩邊取指數：
$\mu(x) = e^{\int P(x),dx}$

結論 Conclusion：

積分因子為：

 $\mu(x) = e^{\int P(x)dx}$

 The integrating factor is: $\mu(x) = e^{\int P(x),dx}$

---




