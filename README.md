# suzuki-book-errata

[in Japanese]  
  
鈴木英男: 整数論・暗号理論・符号理論:PARI/GPで計算しながら学ぶ, 近代科学社, ISBN:9784764907577.  
https://www.kindaikagaku.co.jp/book_list/detail/9784764961159/  
https://www.amazon.co.jp/dp/4764907577/  
の  
2025.8.29版 Ver.1.0 正誤表  
  
p.5  
誤  
raed( "プログラムファイル名" )  
正  
read( "プログラムファイル名" )  
  
p.49  
誤  
1個の解x   
d個の解x  
正  
1個の解$x$   <-- TeXソース  
d個の解$x$   <-- TeXソース  

p.56 下のstep 1  
誤  
MALL=1;  
for(i=1,3,MALL = MALL * m[i])  
正  
MALL=1;  
for(i=1,length(m),MALL = MALL * m[i])  
  
p.56 下のstep 2  
誤  
M = vector(3);  
for(i=1,3,M[i] = MALL / m[i]); M  
正  
M = vector(length(m));  
for(i=1,length(m),M[i] = MALL / m[i]); M  
  
p.57 1,2行目  
誤  
MINV = vector(3);  
for(i=1,3,MINV[i] = lift( Mod(M[i], m[i])^-1 )); MINV  
正  
MINV = vector(length(m));  
for(i=1,length(m),MINV[i] = lift( Mod(M[i], m[i])^-1 )); MINV  
  
p.57 step 4  
誤  
MMINV = vector(3);  
for(i=1,3,MMINV[i] = lift(Mod(M[i] * MINV[i], MALL))); MMINV  
正  
MMINV = vector(length(m));  
for(i=1,length(m),MMINV[i] = lift(Mod(M[i] * MINV[i], MALL))); MMINV  
  
p.60   
誤  
[問1.12.4]  
正  
[問1.12.4]\(解法(3)で解く\) 

p.62 下から9行目  
誤  
Pol(b)  
正  
kill(x); Pol(b)  
  
p.62 下から6行目  
誤  
lift(lift(Mod(Mod(Pol(b),x^7-x),7)))  
正  
lift(lift(Mod(Mod(eval(Pol(b)),x^7-x),7)))  
  
p.68 §1.14.1 の下から4行目  
誤  
最大位奇数    
正  
最大位数  
  
p.109 下から8行目  
誤  
ガロア体$¥mathbb{F}_{2^3}$のための     <-- TeXソース  
正  
ガロア体$¥mathbb{F}_{2^4}$のための     <-- TeXソース  
  
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
  
p.197 脚注 15  
誤  
https://www.ipa.go.jp/security/pki/084.html  
正  
https://web.archive.org/web/20200130073335/https://www.ipa.go.jp/security/pki/084.html  
  
p.241 (3.2.4)式  
誤  
1 \leq    <-- TeXソース  
正  
0 \leq    <-- TeXソース  
  
p.241 (3.2.5)式  
誤  
1 \leq    <-- TeXソース  
正  
0 \leq    <-- TeXソース  
  
p.246 17,18行目  
誤  
エントロピー H は  
H=0; for(i=1,4,H -= q[i]*log(q[i])/log(2)); H  
正  
エントロピー H は  
H=0; for(i=1,length(q),H -= q[i]*log(q[i])/log(2)); H  
  
p.247 8,9行目  
誤  
平均符号長 n は  
n=0; for(i=1,4,n+=q[i]*len[i]); n  
正  
平均符号長 n は  
n=0; for(i=1,length(q),n+=q[i]*len[i]); n  
  
p.262 下から2行目  
誤  
≡0-  
正  
≡0  
  
p.289    
誤  
　　　][[step 1]]  
正  
[step 1]  
  
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
  
p.311 [A.2.11]  
誤  
if,while,until,forでは条件式aが真のときseqを処理する.   
正  
if,while,forでは条件式aが真のときseqを処理する. untilでは条件式aが偽のときseqを処理する.   
  
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
  
p.344 [Ubuntu (Linux) 用sagemath package(pkg) のinstall]の下  
誤  
aptコマンド...の行から  
5. の行まで  
  
正  
1.  https://doc.sagemath.org/html/en/installation/index.html  
    の  
    Linux  
    の  
    No development  
    の項目を参照  

p.344 下から1行目  
誤  
もし, 3. で  
正  
もし,  

p.345 1〜13行目の行先頭のラベル  
誤  
3b 4b 4c 4d 4e 4f 4g 4h 5  
正  
1 2 3 4 5 6 7 8 9  
に置き換え  
  
p.345 5行目  
誤  
version を調べる.  
正  
version を調べる. 2025年3月時点の最新は {¥tt 10.6} である.  
  
p.345 8行目と9行目の2箇所  
誤  
10.5  
正  
10.6  

p.345 [Windows用]の下の項目 4. の行    
誤  
用の 1,2,3 で  
正  
用の 1 で  
  
p.345 [MacOS用]の下3行分. 4,5行目はそのまま.  
誤  
https://doc.sagemath.org/html/en/installation/index.html の MacOS → No    <-- この行の先頭は 1.  
development:の下にある  
binary build of SageMath をクリックして,     <-- この行の先頭は 2.  
正  
https://github.com/3-manifolds/Sage_macOS/releases で,     <-- この行の先頭は 1.  
最新の version を調べる. 2025年3月時点の最新は {¥tt 10.6} である.  
binary release of SageMath     <-- この行の先頭は 2.  
  
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
  
