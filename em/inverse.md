HIKARI 版・逆運算子法解二階常係數線性微分方程式

表紙 Cover

タイトル / Title: Operator Method for Solving Second-Order Linear Differential Equations
著者 / Author: HIKARI
版型 / Style: 日式簡約風 / Japanese Minimalist Style


---

目次 Table of Contents

1. はじめに / Introduction


2. 基本形式と手順 / Basic Form and Procedure


3. よくある右辺関数の形（Common Forms）


4. 応用トピック / Advanced Topics


5. 例題演算 / Example Problems


6. エラーと修正方法 / Common Mistakes and Fixes


7. 数学記号の英語読み一覧 / English Pronunciations of Math Symbols




---

1. はじめに / Introduction

本筆記では、二階線形常係数微分方程式を逆運算子（逆演算子）を用いて特解を求める方法について、英日対照で簡潔にまとめます。

This note introduces a concise operator method for solving second-order linear differential equations with constant coefficients, focusing on how to find particular solutions.


---

2. 基本形式と手順 / Basic Form and Procedure

対象とする方程式は以下の形です：

L[y] = aD^2 y + bD y + c y = f(x)

これを次のように変形：

y = ⁄L[D] · f(x)

このとき：

D は微分作用素（Differential Operator）

L[D] = aD^2 + bD + c


解法手順 / Procedure

1. 求 L[D] の形


2. 試みて L^{-1}[D] を展開（展開可能な形に分解）


3. 各項へ適用（Common Form 使用）




---

3. よくある右辺関数の形 / Common Forms of f(x)


---

4. 応用トピック / Advanced Topics

A. 共振の場合 / Resonance

もし ，則補助解と重なる → 解が破綻。解決法：

y_p = rac{x}{L'[a]} e^{ax}

B. シフト演算 / Shift Operator

位移特性  を用い、移動された関数にも逆運算子法を適用可能。


---

5. 例題演算 / Example Problems

例題 1：f(x) = e^{2x}

方程式：

y'' - 3y' + 2y = e^{2x}

解：

L[D] = D^2 - 3D + 2

L[2] = 2^2 - 3·2 + 2 = 4 - 6 + 2 = 0 （共振！）


修正：

y_p = rac{x}{L'[2]} e^{2x} = rac{x}{2·2 - 3} e^{2x} = rac{x}{1} e^{2x} = x e^{2x}


---

例題 2：f(x) = \cos(3x)

方程式：

y'' + y = \cos(3x)

L[D] = D^2 + 1

使用虚数展開：


y_p = 	ext{Re} \left( rac{1}{L[3i]} e^{3ix} \right)

L[3i] = -(3^2) + 1 = -9 + 1 = -8

y_p = rac{1}{-8} \cos(3x)


---

6. よくあるエラーと修正法 / Common Mistakes and Fixes


---

7. 数学記号の英語読み一覧 / Pronunciation of Math Symbols


---

End of Note

HIKARIによる制作 / Authored by HIKARI

