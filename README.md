**p2.7**   
식을 만들면 v_1(t)/R = -C * dv_2(t)/dt  
라플라스 transfer를 하면 V_1(s)/R = -Cs * V_2(s)  
따라서 transfer function은 V_2(s)/V_1(s) = -1/RCs

---

**p2.12**  
Y(s)/R(s) = k/(s+50)  
R(s) = 1/s이므로  
Y(s) = k/50*(1/s - 1/(s+50))  
y(t) = k/50*(1-e^-50t)  
t -> ∞이면 y(t) -> k/50 = 1이므로  
k = 50  

---

**p2.15**  
mx''(t) + bx'(t) + kx(t) = 0  
x''(t) + (b/m)x'(t) + (k/m)x(t) = 0  
라플라스로 변환하면  
s^2X(s) - sx(0) - x'(0) + b/m(sX(s) - x(0)) + k/m*X(s)  
(s^2+bs/m+k/m)X(s) = x'(0)이므로  
X(s) = x'(0)/(s^2+bs/m+k/m)  
x(t) = b/2m $\cos($$\sqrt{(k/m)-(b^2/4m^2)}$$)$

---


**p2.26**  
Mx''(t) + b(x'(t)-y'(t)) + k(x(t) - y(t)) = F(t)  
my''(t) + b(y'(t)-x'(t)) + k(y(t)-x(t)) = 0  

Laplace transform을 구하고 matrix로 나타내면    
$\begin{bmatrix}Ms^2 + bs + k&-(bs+k)\\-(bs+k)&ms^2 + bs + k\\ \end{bmatrix}$ *
$\begin{bmatrix}X(s)\\Y(s)\\ \end{bmatrix}$
= $\begin{bmatrix}F(s)\\0\\ \end{bmatrix}$  


Y(s)/F(s) = (1/mM(bs+k))/[s^2{s^2+(1+m/M)(bs/m+k/m)}]

---

**p2.37**  
m_1 * (d^2)x/dt^2 = -(k_1 + k_2)x - k_2 * y  
m_2 * (d^2)y/dt^2 = k_2 * (x - y) + u  

m1 = m2 = 1 이고 k1 = k2 = 1이므로  
(d^2)x/dt^2 = -2x - y , (d^2)y/dt^2 =  x - y + u  

<!---
kmjw99/kmjw99 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
