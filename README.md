# suzuki-book-errata

[in Japanese]  
  
鈴木英男: 整数論・暗号理論・符号理論:PARI/GPで計算しながら学ぶ, 近代科学社, ISBN:9784764907577.  
https://www.kindaikagaku.co.jp/book_list/detail/9784764961159/  
https://www.amazon.co.jp/dp/4764907577/  
の  
2025.8.29版 Ver.1.0 正誤表  
  
p.325  
誤  
https://github.com/hideo7suzuki/parigp-h7s-functions/h7s-functions.gp  
正  
https://github.com/hideo7suzuki/parigp-h7s-functions/blob/main/h7s-functions.gp  
  
p.334  
誤  
https://github.com/hideo7suzuki/parigp-h7s-AES/h7s-AES.gp  
正  
https://github.com/hideo7suzuki/parigp-h7s-AES/blob/main/h7s-AES.gp  
  
p.49  
誤  
1個の解x   
d個の解x  
正  
1個の解$x$   
d個の解$x$  

p.68 §1.14.1 の下から4行目  
誤  
最大位奇数    
正  
最大位数  
  
p.143 下から7行目  
誤  
|  p  |  
正  
|p|  
  
p.175 3行目  
誤  
p.218  
正  
p.209  
  
p.181 10行目  
誤  
1254^11 = (F) × (B) =   
正  
1254^11 = (F) × (R) =    

p.262 下から2行目  
誤  
≡0-  
正  
≡0  
  
p.290 [step 4]を次に置き換え  
正  
X=matrix(16,7);  
for(i=1,16,X[i,] = Vecrev(Vecrev(X2[i],7)))  
X  
  
% =   
[0 0 0 0 0 0 0]  
[0 0 0 1 0 1 1]  
[0 0 1 0 1 1 0]  
[0 0 1 1 1 0 1]  
[0 1 0 0 1 1 1]  
[0 1 0 1 1 0 0]  
[0 1 1 0 0 0 1]  
[0 1 1 1 0 1 0]  
[1 0 0 0 1 0 1]  
[1 0 0 1 1 1 0]  
[1 0 1 0 0 1 1]  
[1 0 1 1 0 0 0]  
[1 1 0 0 0 1 0]  
[1 1 0 1 0 0 1]  
[1 1 1 0 1 0 0]  
[1 1 1 1 1 1 1]  
  
p.345 8行目と9行目の2箇所  
誤  
10.5  
正  
10.6  

p.367  
誤  
[Lenstra2]]  
正  
[Lenstra2]  
  
p.368 [Melchor 他]   | 削除  
誤  
https://pqc-hqc.org/|  
正  
https://pqc-hqc.org/  
  
p.372 [Shoup]   | 削除  
誤  
https://www.shoup.net/|  
正  
https://www.shoup.net/  
  
p.374 [WEF]   | 削除  
誤  
https://jp.weforum.org/publications/the-next-generation-of-data-sharing-|...  
正  
https://jp.weforum.org/publications/the-next-generation-of-data-sharing-...  
  
p.376  
誤  
GCM (Galois/counter) モード ......... 175  
GCM (Galois/counter) モード ......... 209  
正  
GCM (Galois/counter) モード ..... 175,209  
  
