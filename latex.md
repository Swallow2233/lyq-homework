# LaTeX

$a_{1}$<br/>
$x^{2}$<br/>
$e^{-\alpha t}$<br/>
$a^{3}_{ij}$<br/>
$e^{x^2} \neq {e^x}^2$<br/>

$\sqrt{x}$<br/>
$\sqrt{x^{2}+\sqrt{y}}$<br/>
$\sqrt[3]{2}$<br/>
$\surd[x^2+y^2]$<br/>

$\overline{m+n}$<br/>
$\underline{m+n}$<br/>

$\underbrace{a+b+\cdots+z}_{26}$<br/>

$\vec a$<br/>
$\overrightarrow{AB}$<br/>

$1\frac{1}{2}$~hours<br/>

$\frac{x^{2}}{k+1}$<br/>
$x^{\frac{2}{k+1}}$<br/>
$x^{1/2}$<br/>

$\sum_{i=1}^{n}$<br/>
$\int_{0}^{\frac{\pi}{2}}$<br/>
$\prod_\epsilon$<br/>


# 十进制转化其他进制——取余法的证明

首先，我们给出一个十进制数N，要求转化为i进制。  
我们可以写出  

$\qquad \qquad N=c_{1}*i^{0}+c_{2}*i^{1}+\cdots+c_{n}*i^{n-1}$  

对于$c_{j}(j=1,2,\cdots,n)$    
若$c_{j}>=i$，则一定存在一个实数$k<i$，使得$k+m*i=c_{j}$  
那么  
$\qquad c_{j}*i^{j-1}+c_{j+1}*i^{j}$<br/>
$=(k+m*i)*i^{j-1}+c_{j+1}*i^{j}$<br/>
$=k*i^{j-1}+m*i^{j}+c_{j+1}*i^{j}$<br/>
$=k*i^{j-1}+(c_{j+1}+m)*i^{j}$<br/>

让$k$作为新的$c_{j}$，$c_{j+1}+m$作为新的$c_{j+1}$。  
以此类推，对于任意的$c_{j}(j=1,2,\cdots,n)$一定有$c_{j}<i$

给等式右边提出公因式$i$，可以得到：  
$N=(c_{2}*i^{1-1}+c_{3}*i^{2-1}+\cdots+c_{n}*i^{n-1-1})*i+c_{1}$

即  $c_{1}=N\quad mod\quad i$   
以此类推，任意的$c_{j}(j=1,2,\cdots,n)=N \quad mod \quad i^{j}.$  

由位置表示法可知，对于任意一个$i$进制的数，$c_{n}$为其第n位数，$c_{n}<i$，令其转化为十进制数N时：  
$\\\qquad \qquad c_{n}*i^{n-1}+c_{n-1}*i^{n-2}+\cdots+c_{1}*i^{0}=N$  

因此，我们可以通过取余的操作得到每一位的$c_{n}$.

综上，十进制转化为其他进制的取余法是成立的。  
证毕！
