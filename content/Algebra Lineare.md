# Indice
[[#Strutture Algebriche]]
[[#Matrici]]
[[#Spazi Vettoriali]]
[[#Applicazioni Lineari]]



---

# Strutture Algebriche
Gli insiemi numerici principali sono i seguenti:
$$
Z = \{0, \pm1,\pm2,\pm3,...\pm n\}
$$
$$
Q=\{\frac{m}{n}| m \in Z , n\in Z, n \neq0\}
$$
$$
R=\{M,C_1,C_2....C_{\infty}|M\in Z, C_{i}\in Z, 0 \leq C_{i} \leq 9\}
$$
Noi sappiamo che su questi insiemi possiamo fare due operazioni:
- SOMMA -> $2 + 3 = 5$
- PRODOTTO -> $2 \times 3 = 6$ 
Quindi, un'operazione è una funzione che ad una coppia di numeri associa un altro numero.
## **DEFINIZIONE** (PRODOTTO CARTESIANO)
siano $A \ e \ B$  due insiemi; si chiama prodotto cartesiano di A per B, L'insieme:
$A \ X \ B \ = \{ (a,b)| \ a \in A, \ b \in B\}$
## **ESEMPIO**
sia  $A= \{ 1,2 \}, \ B= \{2,3,4 \}$
$A \ X \ B = \{(1,2),(1,3),(1,4),(2,2),(2,3),(2,4) \}$
## **DEFINIZIONE** (OPERAZIONE BINARIA INTERNA)
sia A un insieme qualunque.
si chiama ==operazione binaria interna== su A una funzione
$A \ X \ A \to A$
### NOTAZIONE
sia $(a,b \in  A \ X \ A; \ f((a,b)) \in A)$
indicheremo l'operazione con $*$ e scriveremo:
$a*b=f((a,b))$
## **DEFINIZIONE** (STRUTTURA ALGEBRICA)
si chiama ==struttura algebrica== un insieme su cui sono definite una o più operazioni
## **DEFINIZIONE** (GRUPPOIDE)
si chiama ==Gruppoide== una struttura algebrica costituita da un insieme A e da una operazione binaria interna su A, e scriviamo $(A,*)$
## **DEFINIZIONE** (PROPRIETA' ASSOCIATIVA)
sia $(A,*)$ un gruppoide. 
diremo che l'operazione $*$ gode della proprietà associativa se
$(a*b)*c=a*(b*c)$ , $\forall a,b,c \in A$ 
## ESEMPIO
$(2 \times 3)\times 4=6 \times 4=24$ $\equiv$ $2 \times (3 \times 4)=2 \times 12 = 24$ 
$(2+3)+4=5+4=9$ $\equiv$ $2+(3+4)=2+7=9$
## **DEFINIZIONE** (SEMIGRUPPO)
sia $(A,*)$ un gruppoide. 
diremo che $(A,*)$ è un semigruppo se l'operazione è associativa.
## **DEFINIZIONE** (ELEMENTO NEUTRO)
sia $(A,*)$ un gruppoide. 
sia $\epsilon \in A$, diremo che che $\epsilon$ è un elemento neutro se 
$a*\epsilon =\epsilon*a=a$,   $\forall a \in A$
## PROPOSIZIONE
sia $(A,*)$ un gruppoide.
siano $\epsilon$ ,$\epsilon ^I$ $\in A$.
elementi neutri $\rightarrow$ $\epsilon = \epsilon ^I$
### DIMOSTRAZIONE
$\epsilon*\epsilon ^I=\epsilon$                          $\epsilon ^I*\epsilon=\epsilon^I$
quindi $\epsilon=\epsilon ^I$
## **DEFINIZIONE** (MONOIDE)
sia $(A,*)$ un semigruppo. 
diremo che esso è un monoide se esiste l'elemento neutro.
## ESEMPIO 
$(Z, +)$ è un monoide con elemento neutro 0.
$(Z, \times)$ è un monoide con elemento neutro 1.
## **DEFINIZIONE** (INVERTIBILITA')
sia $(A,*)$ un monoide, con elemento neutro $\epsilon$ .
sia $a \in A$  diremo che $a$ è invertibile se $\exists a^{*}\in A$ , tale che
$a*a^{*}=a^{*}*a=\epsilon$
in questo caso diremo che $a^*$ è un inverso di a.
## ESEMPIO
(1) consideriamo il monoide $(Z, +)$ sia $2 \in Z$
2 è invertibile.
infatti $2+(-2)=(-2)+2=0$
(2) consideriamo il monoide $(Z, \times)$ sia $2 \in Z$
2 non è invertibile.
(3) consideriamo il monoide $(Q, \times)$, sia $2 \in Q$ 
2 è invertibile.
infatti $2 \times \frac{1}{2}=\frac{1}{2}\times 2=1$ 
## PROPOSIZIONE
sia $(A,*)$ un monoide. sia $a \in A$, $a$ invertibile $\rightarrow$ $a$ ha solo un inverso.
#### *DIMOSTRAZIONE*
siano $a^{*}\in A$ e $a^{**}\in A$ due inversi di A.
-  $(a^{*}* a)*a^{**}=a^{*}*(a*a^{**})$
-  $(a^{*}*a)*a^{**}=\epsilon * a^{**}=a^{**}$ 
- $(a^{**}*a)*a^{*}=\epsilon * a^{*}=a^{*}$
si ricava che $a^{*}=a^{**}$
## PROPOSIZIONE 
sia $(A, *)$ un monoide. siano $a \in A, b \in A$, due elementi invertibili.
siano $a^{-1}$ e $b^-1$ gli inversi di $a$ e $b$ rispettivamente.
allora $a*b$ è invertibile e 
$(a*b)^-1=b^{-1}*a^{-1}$ 
#### DIMOSTRAZIONE
vogliamo dimostrare che $b^{-1}*a^-1$ è l'inverso di $a*b$ .
infatti:
- $(a*b)*(b^{-1}*a^{-1})=a*(b*b^{-1})*a^{-1} \ =(a*\epsilon)*a^-1=a*a^-1=\epsilon$ 
- $(b^{-1}*a^{-1})*(a*b) =b^{-1}*(a^{-1}*a)*b=(b^{-1}*\epsilon)*b=b^{-1}*b=\epsilon$ 
## NOTAZIONE 
sia $(A,*)$ un monoide, sia $a \in A$ invertibile.
denoteremo l'inverso di a con il simbolo $a^{-1}$
## **DEFINIZIONE** (GRUPPO)
si chiama gruppo un monoide nel quale ogni elemento è invertibile.
## **DEFINIZIONE** (PROPRIETA' COMMUTATIVA) 
sia $(A,*)$ un gruppoide.
diremo che l'operazione $*$ gode della proprietà commutativa se 
$a*b=b*a$  $\forall a,b \in A$ 
## **DEFINIZIONE** (GRUPPO ABELIANO)
un gruppo $(A,*)$ si dice Abeliano se l'operazione è commutativa.
### ESEMPIO
- $(Z, +)$ è un gruppo abeliano
- $(Z, \times)$ è un monoide, ma non un gruppo
- $(Q, \times)$ è un monoide, ma non è un gruppo
- $(Q \{0\}, \times)$ è un gruppo abeliano
- $(R\{0\}, \times)$ è un gruppo abeliano
- $(Q, +)$ è un gruppo abeliano
- $(R,+)$ è un gruppo abeliano

## **DEFINIZIONE** (ANELLO)
sia $(A,*, \times)$ una struttura algebrica.
diremo che essa è un anello se valgono le seguenti proprietà:
- $(A,+)$ è un gruppo abeliano
- $(A, \times)$ è un semigruppo
- proprietà distributiva rispetto alla somma
## NOTAZIONE
sia $(A,+,\times)$ un anello.
l'elemento neutro della somma lo indichiamo con 0 e lo chiamiamo zero.
$\forall a \in A$, il suo inverso rispetto alla somma lo indichiamo con $-a$ e lo chiamiamo opposto.
quindi $a+(-a)=(-a)+a=0$ 

## **DEFINIZIONE** (ANELLO UNITARIO)
un anello $(A,+,\times)$ si dice unitario se esiste l'elemento neutro rispetto al prodotto.
lo indichiamo con il simbolo 1 e lo chiamiamo unità.
l'inverso di un elemento $a\in A$, se esiste lo indichiamo con il simbolo $a^-1$. 
## **DEFINIZIONE** (ELEMENTO NEUTRO +)
sia $(A,+, \times)$ un anello. 
	ricordiamo che con 0 indichiamo l'elemento neutro della somma.
## PROPOSIZIONE
sia $(A,+, \times)$ un anello.
$a \times 0=0 \times a=0$    $\forall a \in A$ 

### DIMOSTRAZIONE
$a \times 0=a \times (0+0)=a \times 0+a \times 0$
$a \times 0=a \times 0 + a \times 0 \rightarrow$
$\ a \times 0 +(-a \times 0)=a \times 0+(a \times 0+(-a \times 0)) \rightarrow$
$0=a \times 0+0 \rightarrow$
$0=a \times 0$
quindi si prova che $0 \times a=0$
## NOTAZIONE
sia $(A,+,\times)$ un anello unitario
sia $a \in A$ invertibile rispetto al prodotto.
denoteremo il suo inverso con $a^-1$, quindi
$a \times a^-1=a^-1 \times a=1$
### ESEMPIO
$(Z,+,\times)$ è un anello unitario.
gli unici elementi invertibili rispetto al prodotto sono 1 e -1.
ovviamente $1^-1=1 \ \ \ (-1)^-1=-1$
## OSSERVAZIONE
sia $(A,+, \times)$ un anello unitario.
0 è invertibile rispetto al prodotto?

$0 \times x =1 \rightarrow 0=1$ può accadere solo se i due elementi neutri coincidono.
ma quando $0=1?$ $a \in A$, se $0=1$ , $a \times 0=0$, $a \times 1=a$ $\rightarrow$ 
$\rightarrow a \times 0=a \rightarrow a=0$ $\equiv$ $a \times 1=0 \rightarrow a=0 \rightarrow A=\{0\}$
quindi l'elemento neutro della somma è invertibile rispetto al prodotto solo se $A$ contiene solo $0$ 
## **DEFINIZIONE** (CORPO E CAMPO)
un anello unitario si chiama corpo se tutti i suoi elementi non nulli sono invertibili rispetto al prodotto .
un corpo si chiama campo se il prodotto è commutativo.

### ESEMPI
- (1) CAMPO DEI NUMERI RAZIONALI
  $(Q,+,\times)$ è un campo
-  (2) CAMPO DEI NUMERI REALI
   $(R,+,\times)$ è un campo
- $(Z,+,\times)$ è un anello unitario, ma non è un corpo.
## **DEFINIZIONE** (CAMPO DEI NUMERI COMPLESSI)
sia $C=R^2=R \ X \ R$
definiamo su $C$ le due operazioni
- SOMMA 
  $siano \ (a,b),(c,d)\in C$
  $(a,b)+(c,d)=(a+c,b+d)$
- PRODOTTO
  $siano (a,b),(c,d)\in C$
  $(a,b)\times(c,d)=(ac-bd,ad+bc)$
### ESEMPIO
$(1,3)+(2,5)=(3,8)$
$(1,3)\times (2,5)=(1\times 2-3\times 5, 1\times 5 +3 \times 2=(-13,11)$

- (1) $(C,+)$ è un gruppo abeliano
  con elemento neutro $(0,0);\ \ \forall (a,b)\in C \ \ \ -(a,b)=(-a,-b)$
- (2) il prodotto è associativo (DA VERIFICARE)
- (3) valgono le proprietà distributive (DA VERIFICARE)
- (4) $(1,0)$ è l'elemento neutro del prodotto
  $(a,b)\times(1,0)=(a\times 1-b\times 0, a\times 0+b \times 1)=(a,b)$
  $(1,0)\times (a,b)=(1 \times a - 0 \times b, 1 \times b+0 \times a)=(a,b)$
- (5) sia $(a,b)\in C$  , $(a,b)\neq(0,0)$ 
  dobbiamo risolvere l'equazione $(a,b)\times(x,y)=(1,0) \rightarrow$ 
  $(ax-by+ay-bx)=(1,0)$

  $\begin{cases} ax-by=1 \\ ay+bx=0  \end{cases} \rightarrow$ $\begin{cases} ax-by=1 \\ y=-\frac{b}{a}x \end{cases}\rightarrow$ $\begin{cases}ax -b\left( -\frac{b}{a}x \right)=1 \\ y=-\frac{b}{a}x \end{cases}$
  $\begin{cases}ax -\frac{b^2}{a}x=1 \\ y=-\frac{b}{a}x\end{cases}\rightarrow$ $\begin{cases}a^2x-b^2x=a \\ y=-\frac{b}{a}x  \end{cases}\rightarrow$ $\begin{cases} (a^2+b^2)x=1  \\ y=-\frac{b}{a}x \end{cases}$
  $\begin{cases}x=\frac{a}{(a^2+b^2)} \\y=-\frac{b}{a}x  \end{cases} \rightarrow$ $\begin{cases}x=\frac{a}{(a^2+b^2)}\\ y=-\frac{b}{a} \frac{a}{(a^2+b^2)} \end{cases} \rightarrow$ $\begin{cases}x= \frac{a}{(a^2+b^2)} \\ y=-\frac{b}{(a^2+b^2)}\end{cases}\rightarrow$ 
  abbiamo dimostrato che  $(a,b)^-1=\left( \frac{a}{(a^2+b^2)}, \frac{b}{(a^2+b^2)} \right)$ 
  - (6) la moltiplicazione è commutativa

  ### **FORMA ALGEBRICA DI UN NUMERO COMPLESSO**
  poniamo $i=(0,1)$
 
  ### PROPOSIZIONE 
  $i^2=-(1,0)$

  #### DIMOSTRAZIONE
  $(0,1)\times(0,1)=(0-1,0+0)\rightarrow$
  $(-1,0)\rightarrow-(1,0)$

  ## NOTAZIONE
  i numeri complessi possono essere rappresentati sul piano cartesiano:
  ![[Drawing 2025-10-08 21.09.51.excalidraw]]
  ogni elemento dell'asse x corrisponde ad un numero reale:
  $(a,0),a\in A$          $R\subset C$ 
## **DEFINIZIONE** (a+bi)
$a+bi$ si chiama forma algebrica del numero complesso
## **DEFINIZIONE** 
sia $z\in C$, $z=a+ib$ , si chama coniugato di Z il numero
$z^==a-ib$ 
si chiama modulo di $z$ il numero
$|z|=\sqrt{ a^2+b^2 }$ 
si chiama parte reale di $z$, il numero reale
$Re \ z=a$
si chiama parte immaginaria di $z$, il numero reale
$Im \ z=b$
![[Drawing 2025-10-08 22.08.48.excalidraw]]
## PROPOSIZIONE
$sia \ z\in C$
$z \in R \leftarrow\rightarrow z=z^=$ 
### DIMOSTRAZIONE 
sia $z=a+bi$              $z \in R \leftarrow\rightarrow b=0\leftarrow\rightarrow z=a \leftarrow\rightarrow z^==a=z$ 
## PROPOSIZIONE
sia $z\in C$
- (1) 
  $z\times z^==|z|^2$ 
- (2)
  se $z \neq 0$ ,    $z^-1=\frac{z^=}{|z|^2}$ 
### DIMOSTRAZIONE
- (1) sia $z=a+bi$ ; $z^==a-bi$ 
  $z\times z^{=}=(a+bi)(a-bi)=a^2-abi+abi-b^2i^2=a^2+b^2i^2=a^2+b^2 \rightarrow z\times z^==|z|^2$    
## PROPOSIZIONE 
sia $z \in C$,  $z\not\in R$  
$z \ e \ z^=$  sono soluzioni di una equazione di secondo grado a coefficienti reali
### DIMOSTRAZIONE
$(x-z)(x-z^=)=x^2-(z+z^=)x+z\times z^=$
sia $z=a+bi$;   
$x^{2}-(a+bi+a-bi)x+|z|^2\rightarrow$ $x^{2}-2(Re \ z)+ |z|^2$ 

### ESEMPIO
sia $z=2+3i$ 
allora $x^{2}-2(2)x+13\rightarrow x^2-4x+13=0$
quindi $z$ è soluzione dell'equazione, infatti:
$\frac{\Delta}{4}=4-13=-9$ $\rightarrow$ $\sqrt{-9}=\sqrt{(-1)\times 9}=\sqrt{-1}\times \sqrt{9}=3i$ 
$x=\frac{4\pm 3i}{2}$ $\rightarrow$ $x=2\pm 3i$ 

# Matrici
sia $(K,+,\times)$ un campo (per esempio $K=R$).
siano $m \in Z, n \in Z, \ m>0, n>0$
sia $I=\{1,2,....,n\}$ e $J=\{1,2,....,n\}$
## **DEFINIZIONE**  (MATRICE)
si chiama matrice con m righe ed n colonne ad elementi in K una funzione:
$I \ X \ J \rightarrow K$
### NOTAZIONE
per rappresentare una matrice utilizziamo una tabella con m righe e n colonne

$M= \begin{vmatrix} a_{11} \ \ a_{12} \ \ a_{13} \ \ a_{14} \\ a_{21}\ \ a_{22} \ \ a_{23} \  \  a_{24} \\ a_{31} \ \ a_{32} \ \ a_{33} \ \ a_{34}\end{vmatrix}$
con $a_{ij}$
in questo caso $m=3 \ e \ n=4$
## NOTAZIONE
poniamo $K^{m,n}=insieme \ di\ tutte\ le\ matrici\ con\ m\ righe\ ed\ n\ colonne\ ad\ elementi\ in\ K$

### ESEMPIO
sia $A=\begin{vmatrix} 2  &  3 &  4\\ 1  &  5  &  1    \end{vmatrix} \in R^{2,3}$

sia $B=\begin{vmatrix}1  &  5  &  2+3i  &  7 \\ 7  &  i  &  4  &  -2 \end{vmatrix} \in C^{2,4}$

## NOTAZIONE
sia $M\in K^{m,n}$. 
poniamo $ent_{ij}=l'elemento \ situato \ sulla \ riga \ i \ e \ colonna \ j  \ della \ matrice \ M$
quindi $ent_{ij}\in K$
### ESEMPIO 
sia $M= \begin{vmatrix} 3 & 8 & 9 & 6 & 3 \\ 2 & -1 & 4 & 1 & 0 \\ 5 & 6 & 2 & 1 & 2               \end{vmatrix} \in R^{3,5}$
$ent_{2,4}(M)=1$

## **DEFINIZIONE** (SCALARI)
gli elementi del campo K si chiamano *scalari*
## **DEFINIZIONE** (Elementi)
siano $A \in K^{m,n}, B\in K^{m,n}$
definiamo $A+B \in K^{m,n}$
$ent_{ij}(A+B)=ent_{ij}(A)+ent_{ij}(B)$

### ESEMPIO
siano $A=\begin{vmatrix}1 & 0 & 3 \\ 2 & 4 & 5  \end{vmatrix} \in R^{2,3}$; $B=\begin{vmatrix}4 & 6 & -1 \\ 3 & 1 & 8\end{vmatrix} \in R^{2,3}$

$A+B=\begin{vmatrix}5 & 6 & 2 \\ 5 & 5 & 13 \end{vmatrix}$

## PROPOSIZIONE
$(K^{m,n},+)$ è un gruppo abeliano.
- l'operazione è binaria interna 
- l'operazione è associativa $\rightarrow$ $(A+B)+C=A+(B+C)\ \ \ \forall A,B,C \in K^{m,n}$
- esistenza dell'elemento neutro $\rightarrow$ $A+0=0+A=A$    $\forall A\in K^{m,n}$
- esistenza dell'inverso
- l'operazione è commutativa

### ESEMPIO
sia $A=\begin{vmatrix} 2 & 3 & -5 \\ 4 & 2 & 8 \\ 7 & -6  & -2 \\ 4 & 1 & 3     \end{vmatrix} \in R^{4,3}$;          sia $-A=\begin{vmatrix}-2 & -3 & 5 \\ -4 & -2 & -8 \\ -7 & 6 & 2 \\ -4 & -1 & -3     \end{vmatrix} \in R^{4,3}$

$A+(-A)=0$

## **DEFINIZIONE** (PRODOTTO DI UNO SCALARE PER UNA MATRICE)

sia $(K,+,\times)$ un campo e siano $a \in K$ e $M \in K^{m,n}$ 
vogliamo definire una matrice $a\times M \in K^{m,n}$ nel seguente modo
$$ent_{ij}(a\times M)=a \times ent_{ij}(M)$$

### ESEMPIO
sia $M=\begin{vmatrix}5 & 1 & -6 \\ -3 & 2 & 0 \end{vmatrix} \in R^{2,3}$ ,   $a=3 \in R$

$a \times M=3 \begin{vmatrix}5 & 1 & -6 \\ -3 & 2 & 0 \end{vmatrix}= \begin{vmatrix} 15 & 3 & -18 \\ -9 & 6 & 0   \end{vmatrix} \in R^{2,3}$
### OSSERVAZIONE
il prodotto di uno scalare per una matrice è una operazione del tipo:
$K\ X \ K^{m,n} \rightarrow K^{m,n}$

#### PROPRIETA'
sia $(K,+, \times)$ un campo.
- $(a+b)\times M=a\times M + b\times M$              $\forall a,b \in K, \ \ \forall M \in K^{m,n}$
- $a \times (M+N)=a\times M +a\times N$            $\forall a \in K, \ \ \forall M,N \in K^{m,n}$
- $a\times(b\times M)=(a\times b)\times M$                     $\forall a,b \in K, \ \ \forall M \in K^{m,n}$
- $1 \times M=M$                                                 $\forall M \in K^{m,n}$

## **DEFINIZIONE** (PRODOTTO TRA MATRICI)
sia $(K,+,\times)$ un campo e siano $A \in K^{m,n}, \ \ A \in K^{m,n}$
definiamo il prodotto $A\times B \in K^{m,n}$
$ent_ij(A\times B)=\sum_{r=1}^{n}ent_{ij}(A)\times ent_{ij}(B)$

### ESEMPIO
$A=\begin{vmatrix} 2 & 3 & 1 \\ 4 & 1 & 2    \end{vmatrix} \in R^{2,3}$;     $B=\begin{vmatrix} 1 & -1 & 2 & 1 \\ 3 & 2 & 1 & 0 \\ 2 & 1 & 4 & 1    \end{vmatrix} \in R^{3,4}$

$ent_{ij}11=2\times 1+3\times 3+1\times 2= 13$
$ent_{ij}21=4\times 1+1\times 3+2 \times 2=11$

$A\times B= \begin{vmatrix}13 & 5 & 11 & 3 \\ 11 & 0 & 17 & 6    \end{vmatrix}$
### PROPRIETA'
- $(A\times B)\times C=A\times(B\times C)$                       $\forall A\in K^{m,n}, \forall B\in K^{m,p}, \forall C \in K^{n,q}$
- $A\times(B + C)= A\times B+A \times C$                  $\forall A\in K^{m,n}, \ \ \ \forall B,C \in K^{n,p}$
- $(a\times M)\times N=a\times (M\times N)=M\times(a\times N)$     $\forall a \in K,\ \ \forall M \in K^{m,n}, \ \forall N \in K^{n,p}$
### OSSERVAZIONE
non sempre vale la proprietà commutativa.
sia $A=\begin{vmatrix}1 & 0 \\ 0 & 0     \end{vmatrix} \in K^{2,2}$ ,   $B=\begin{vmatrix}0 & 1 \\0 & 0     \end{vmatrix} \in K^{2,2}$

$A \times B= \begin{vmatrix} 0 & 1 \\ 0 & 0     \end{vmatrix}= B$
$B \times A=\begin{vmatrix} 0 & 0 \\ 0 & 0    \end{vmatrix}=0$
$A\times B \neq B\times A$

#### ESERCIZIO
definire l'insieme delle matrici $R^{2,2}$ che commutano con $A=\begin{vmatrix} 1 & 0 \\ 0 & 0    \end{vmatrix}$.
$X=\begin{vmatrix} x & y \\ z & t    \end{vmatrix}$

$A \times X=$ $\begin{vmatrix} x  & y \\ 0 & 0    \end{vmatrix}$
$X\times A=$ $\begin{vmatrix}x & 0 \\ z &  0     \end{vmatrix}$
$SOLUZIONE=\begin{cases}x=x\\ y=0 \\ z=0 \\ 0(t)=0 \end{cases}$ $\rightarrow$ $X_{sol}=x\begin{vmatrix}x & 0 \\ 0 &  0     \end{vmatrix}$ +  $t\begin{vmatrix}0 & 0 \\0  & t   \end{vmatrix}$    $\forall x,t \in R$ $\rightarrow$ LA SOLUZIONE è $X_{sol}=\begin{vmatrix}x & 0 \\ 0 & t \end{vmatrix}$

## **DEFINIZIONE** (MATRICE QUADRATA)
sia $A \in K^{m,n}$.
diremo che $A$ è una matrice quadrata se $m=n$.

### OSSERVAZIONE
il prodotto di matrici in $K^{n,n}$ è una operazione binaria interna

## PROPOSIZIONE
$(K^{n,n},+,\times)$ è un anello unitario $\forall n  \geq 1$ 
## DIMOSTRAZIONE
dobbiamo dimostrare che il prodotto ha l'elemento neutro.
l'elemento neutro per il prodotto è la matrice:
$I=\begin{vmatrix}1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1     \end{vmatrix}$

dobbiamo dimostrare che $AI=IA=A$
$ent_{ij}(AI) =\sum_{r=1}^{n}ent_{i,r}(A)\times ent_{r,j}(I)$ $\rightarrow$ $ent_{i,j}(A)\times ent_{j,j} (I)$ $= ent_{i,j}(A)$
$AI=A$
$ent_{ij}=\sum_{r=1}^nent_{i,r}(I)\times ent_{r,j}(A) \rightarrow$ $ent_{i,i}(I)\times ent_{i,j}(A)$ $=ent_{i,j}(A)$
IA=A

QUINDI $AI=IA=A$
### ESEMPIO

se $n=2$     $I=\begin{vmatrix}1 & 0 \\ 0 & 1     \end{vmatrix}$
se $n= 3$     $I=\begin{vmatrix}1 & 0 & 0 \\ 0 & 1 & 0  \\ 0 & 0 & 1     \end{vmatrix}$
### DOMANDA
in $K^{n,n}$ quali matrici sono invertibili rispetto al prodotto?
## OSSERVAZIONE
non tutte le matrici non nulle sono invertibili.
sia $A=\begin{vmatrix}1 & 0 \\ 0 & 0     \end{vmatrix}$ .     A non è invertibile.
infatti sia $B=\begin{vmatrix}0 & 1 \\ 0 & 0     \end{vmatrix}$ sappiamo che
$A\times B=B$    e     $B\times A =0$

se A fosse invertibile esisterebbe l'inversa $A^-1$
$(B\times A)\times A^{-1}=0\times A^-1$ $\rightarrow$ $B\times (A\times A^-1)=0$ $\rightarrow$ $B\times I =0$ 
$\rightarrow$ $B=0$ (FALSO)
## **DEFINIZIONE** (DIAGONALI)
sia $A\in K^{n,n}$
![[Screenshot 2025-10-15 101819.png]]

## **DEFINIZIONE** (TRIANGOLARE SUP e INF)
sia $A\in K^{n,n}$. 
A si dice:
- *TRIANGOLARE SUPERIORE*
  se tutti gli elementi al di sotto della diagonale principale sono nulli, ovvero
  $$ent_{ij}(A)=0 \ \ \  \forall i>j$$
- *TRIANGOLARE INFERIORE*
  se tutti gli elementi al di sopra della diagonale principale sono nulli, ovvero
  $$ent_{ij}(A)=0 \ \ \ \forall i<j$$
![[Screenshot 2025-10-15 102945.png]]
## **DEFINIZIONE** (MATRICE DIAGONALE)
sia $A\in K^{n,n}$. 
A si dice diagonale se è sia triangolare inferiore che triangolare superiore.
![[Screenshot 2025-10-15 103128.png]]
## **DEFINIZIONE** (MATRICE SCALARE)
sia $A \in K^{n,n}$.
A si dice Matrice Scalare se esiste $a\in K$, tale che $A=a\times I$
$S=a\times I=a\times \begin{vmatrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{vmatrix}=\begin{vmatrix}a & 0 & 0 \\ 0 & a & 0 \\ 0 & 0 & a\end{vmatrix}$
### OSSERVAZIONE
MATRICE SCALARE $\rightarrow$ MATRICE DIAGONALE $\rightarrow$ MATRICE TRIANGOLARE

## **DEFINIZIONE** (MATRICE TRASPOSTA)
sia $A \in K^{n,n}$. 
si chiama matrice trasposta di A la matrice $A^{t}\in K^{n,n}$ tale che:
$$ent_{ij}(A^t)=ent_{ji}(A)$$
### ESEMPIO
sia $A=\begin{vmatrix}a & b & c \\ d & e & f  \end{vmatrix}\in K^{2,3}$ $\rightarrow$ $A^{t}=\begin{vmatrix}a & d \\ b & e \\ c & f     \end{vmatrix}\in K^{3,2}$
#### PROPRIETA'
- (1)
  $(A+B)^{t}=A^{t}+B^{t}$ ,   $\forall A,B \in K^{m,n}$
- (2)
  $(a\times M)^{t}=a\times M^{t}$,    $\forall a\in K, \forall M\in K^{m,n}$
- (3)
  $(A\times B)^{t}=B^{t}\times A^{t}$ ,   $\forall A\in K^{m,n}, \forall B\in K^{n,p}$
- (4)
  $(A^{t})^{t}=A$,   $\forall A\in K^{m,n}$
## **DEFINIZIONE** (TRACCIA DI UNA MATRICE QUADRATA)
sia $A\in K^{n,n}$
si chiama Traccia di A la somma degli elementi della diagonale principale, ovvero
$$tr(A)=\sum_{r=1}^{n}ent_{rr}(A)$$
![[Screenshot 2025-10-15 110240.png]]

#### PROPRIETA'
- (1)
  $tr(A+B)=tr(A)+tr(B)$,   $\forall A,B \in K^{n,n}$
- (2)
  $tr(a\times M)=a\times tr(M)$,    $\forall a\in K, \forall M\in K^{n,n}$
- (3)
  $tr(A\times B)=tr(B\times A)$,     $\forall A,B \in K^{n,n}$

### ESEMPIO
sia $A=\begin{vmatrix}a & b \\ c & d \end{vmatrix}$ ,  $B=\begin{vmatrix}e & f \\ g & h  \end{vmatrix}$
$A\times B=\begin{vmatrix}ae+bg & af+bh \\ ce+dg & cf+dh\end{vmatrix}$     $tr(AB)=ae+bg+cf+dh;$

$B\times A=\begin{vmatrix}ea+fc & eb+fd \\ ga+hc & gb+hd\end{vmatrix}$     $tr(BA)=ea+fc+gb+hd$

$$tr(AB)=tr(BA);$$

## **DEFINIZIONE** (FUNZIONI)
siano A e B insiemi.
sia $A\rightarrow B$ una funzione.
$f$ si dice iniettiva se $f(a_1)=f(a_2)\implies a_{1}=a_{2}$ 
$f$ si dice suriettiva se $Im f=B$, ovvero $\forall b\in B, \ \ \exists a\in A$  tale che $f(a)=b$.
$f$ si dice biettiva se è sia iniettiva che suriettiva.
### ESEMPIO
![[Screenshot 2025-10-15 112205.png]]

## **DEFINIZIONE** (PERMUTAZIONE)
sia $A$ un insieme.
si chiama permutazione su $A$ una funzione biettiva $A\rightarrow A$.
se $A=\{1,2,3,....,n\}$, indicheremo con $S_n$ l'insieme di tutte le permutazioni su A.
### ESEMPIO
sia $n=3$,  $A=\{1,2,3\}$ 
gli elementi di $S_3$ sono:
![[Screenshot 2025-10-15 115119.png]]

in generale in $S_n$ ci sono $n!$ permutazioni
$n!=\prod_{r=1}^{n}r$ 

#### ESERCIZIO PER CASA
scrivere tutti gli elementi di $S_4$
tutti gli elementi di $S_4$ sono $4!=24$

### ESEMPIO
sia $(5,1,3,6,4,2)\in S_6$
![[Screenshot 2025-10-15 120137.png]]
![[Screenshot 2025-10-15 120143.png]]
per arrivare alla permutazione fondamentale, abbiamo eseguito 4 scambi, ed essendo 4 un numero pari, diremo che questa è una permutazione di classe pari.

## **DEFINIZIONE** (CLASSE DI UNA PERMUTAZIONE)
sia $\sigma \in S_n$ .
diremo che $\sigma$ è di classe pari se occorrono un numero pari di scambi per trasformarla nella permutazione fondamentale, altrimenti diremo che $\sigma$ è di classe dispari.

## **DEFINIZIONE** (SEGNO DI UNA PERMUTAZIONE)
sia $\sigma \in S_n$.

chiamiamo Segno di una permutazione la funzione: 
$$\begin{cases}1 \ \ s e \ \sigma \ e'\ pari \\ -1 \ se \ \sigma \ e'\ dispari\end{cases}$$
### ESERCIZIO 
calcolare i segni delle permutazioni in $S_3$
$S_{3}$ = $\{(1,2,3),(1,3,2),(3,2,1),(2,1,3),(2,3,1),(3,1,2)\}$
$S_3$=$\{+,-,-,-,+,+\}$
## **DEFINIZIONE** (PRODOTTO DEDOTTO)
sia $A\in K^{n,n}$.      sia $\sigma \in S_n$ .
si chiama prodotto dedotto associato alla permutazione $\sigma$, il prodotto
$ent_{1 \sigma(1)} \times ent_{2 \sigma (2)} \times ent_{n \sigma (n)}$ 
### ESEMPIO
sia $A=\begin{vmatrix}a_{11} & a_{12} & *a_{13}* & a_{14} \\ *a_{21}* & a_{22} & a_{23} & a_{24}  \\ a_{31} & a_{32} & a_{33} & *a_{34}* \\ a_{41} & *a_{42}* & a_{43}& a_{44} \end{vmatrix}$ $\in K^{4,4}$

sia $\sigma =(3,1,4,2)$ $\in S_{4} \implies$ $p\sigma =a_{13}\times a_{21}\times a_{34}\times a_{42}$

## **DEFINIZIONE** (DETERMINANTE DI A)
sia $A\in K^{n,n}$.
si chiama determinante di A lo scalare
$$det A=\sum_{\sigma \in S_{n}}sgn(\sigma)\ p\sigma$$
### ESEMPIO
$n=1$         $\ \ A=(a_{11}) \ \ \ \implies$ $det\ A=a_{11}$
$n=2$         $A=\begin{vmatrix}a_{11} & a_{12} \\ a_{21} & a_{22} \end{vmatrix};$    $S_{2}=\{(1,2),(2,1)\}$;
quindi $det A=p_{1,2}-p_{2,1}=a_{11}\times a_{22}-a_{12}\times a_{21}$
### ESEMPIO
$A=\begin{vmatrix}2 & 3 \\ 4 & 5     \end{vmatrix}$;              $det\ A=2\times 5-3\times 4=10-12=-2$
$n=3$           $A=\begin{vmatrix}a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33} \end{vmatrix}\in K^{3,3}$
$S_{3}=\{(1,2,3),(1,3,2),(3,2,1),(2,1,3),(2,3,1),(3,1,2)\}$ 
$detA=p_{1,2,3}-p_{1,3,2}-p_{3,2,1}-p_{2,1,3}+p_{2,3,1}+p_{3,1,2}$
$=a_{11}a_{22}a_{33}-a_{11}a_{23}a_{32}-a_{13}a_{22}a_{31}-a_{12}a_{21}a_{33}+a_{12}a_{23}a_{31}+a_{13}a_{21}a_{32}$


![[Screenshot 2025-10-15 152102.png]]

### ESEMPIO 
sia $A=\begin{vmatrix}2 & 1 & 1 \\ 1 & 3 & 5 \\ 3 & 2 & 1 \end{vmatrix}$ $S_{3}=\{(1,2,3),(1,3,2),(3,2,1),(2,1,3),(2,3,1),(3,1,2)\}$ 
permutazioni pari=$(1,2,3),(2,3,1)(3,1,2)$
permutazioni dispari=$(1,3,2),(3,2,1),(2,1,3)$
$Det A=2\times3\times1+1\times 5\times 3+1\times 1\times 2-2\times5\times 2-1\times 3\times 3-1\times1\times1$
$DetA=6+15+2-20-9=23-29=-7$ 
### PROPRIETA' (DETERMINANTE)
sia $A\in K^{n,n}\implies A=(C_{1},\dots,C_{n})$ dove $C_{1},\dots, C_{n}$ sono le n colonne della matrice.
quindi $C_{i}\in K^{n,1}, \ per\ 1\leq i\leq n$ .
per esempio consideriamo la matrice
$A=\begin{vmatrix}\frac {1}{4} &2 \frac{3}{1}+3\frac{2}{5}\end{vmatrix}$ 
$C_{2}=2 \frac{3}{1}+3\frac{2}{5}=\frac {6}{2}+\frac{6}{15}=\frac{12}{17}$

## DEFINIZIONE (COMBINAZIONE LINEARE)
siano $a,b \in K$ , $M,N \in K^{m,n}$
l'operazione $a\times M+b\times N$ si chiama COMBINAZIONE LINEARE

----
## DEFINIZIONE (SISTEMA DI CRAMER)
un sistema lineare $AX=B$ si dice sistema di cramer se 
1. $A$ è una matrice quadrata
2. $\det A\neq{0}$

## **TEOREMA DI CRAMER**
un sistema lineare di cramer ha sempre una ed una sola soluzione

### DIMOSTRAZIONE
sia $AX=B$ un sistema di cramer $\implies$ $A$ è quadrata e $\det A \neq 0$ $\implies$ $A$ è invertibile.
 
$A^-1(AX)=A^-1B$  $\implies (AA^-1)X=A^-1B$ $\implies IX=A^-1B$ $\implies X=A^-1B$
proviamo che $X=A^-1B$ è una soluzione:
$A(A^-1B)=(AA^{-1})B=IB=B\implies$ $X=A^-1B$
### ESERCIZIO

$\begin{cases}2x+5y=11 \\ 3x+4y =13   \end{cases}$

#SOLUZIONE

$A=\begin{pmatrix}2 & 5 \\ 3 & 4\end{pmatrix}$    $X=\begin{pmatrix}x \\ y\end{pmatrix}$

$B=\begin{pmatrix}11  \\ 13\end{pmatrix}$

$\det A=8-15=-7 \implies \text{il sistema è di cramer}$

$\begin{pmatrix}2 & 5 \\ 3 & 4\end{pmatrix}\cdot \begin{pmatrix}x \\ y\end{pmatrix}=\begin{pmatrix}11 \\ 13\end{pmatrix}$

$A_{AGG}=A^T_{cof}=\begin{pmatrix}4 & -3 \\ -5 & 2\end{pmatrix}=\begin{pmatrix}4 & -5 \\ -3 & 2\end{pmatrix}$
 $A^{-1}=-\frac{1}{7} \cdot \begin{pmatrix}4 & -5 \\ -3 & 2\end{pmatrix}$
$\begin{pmatrix}4 & -5 \\ -3 & 2\end{pmatrix}\cdot \begin{pmatrix}2 & 5 \\ 3 & 4\end{pmatrix}\cdot\begin{pmatrix}x \\ y\end{pmatrix}=\begin{pmatrix}4 & -5 \\ -3 & 2\end{pmatrix}\cdot \begin{pmatrix}11 \\ 13\end{pmatrix} \implies$
$\begin{pmatrix}-7 & 0 \\ 0 & -7\end{pmatrix}\cdot \begin{pmatrix}x \\ y\end{pmatrix}=\begin{pmatrix}4 & -5 \\ -3 & 2\end{pmatrix}\cdot \begin{pmatrix}11 \\ 13\end{pmatrix}$ 
$\begin{pmatrix}-7 & 0 \\ 0 & -7\end{pmatrix}\cdot \begin{pmatrix}x \\ y\end{pmatrix}=\begin{pmatrix}44-65 \\ -33+26\end{pmatrix}$
$\begin{pmatrix}-7 & 0 \\ 0 & -7\end{pmatrix}\cdot \begin{pmatrix}x \\ y\end{pmatrix}=\begin{pmatrix}-21 \\ -7\end{pmatrix}\implies$ $\begin{cases}-7x=-21 \\ -7y=-7\end{cases}$
$\implies \begin{cases}x=\frac{-21}{7}=3 \\ y=\frac{-7}{-7}=1\end{cases}$
LA SOLUZIONE E' $X=\begin{pmatrix}3 \\ 1\end{pmatrix}$

## REGOLA DI CRAMER
sia $AX=B$ un sistema di cramer.
$A\in K^{n,n}$ 
scriviamo A per colonne, $A=(C_{1}\dots C_{n})$ .
poniamo $$A_{(i)}=(C_{1}\dots C_{i-1} \ B \ C_{i+1}\dots C_{n})$$
(in $A$ sostituiamo la colonna i-esima con la colonna $B$)
allora la soluzione del sistema è $S=\begin{pmatrix}s_{1} \\ . \\ . \\s_{n} \end{pmatrix}$
$$$s_{i}=\frac{\det A_{i}}{\det A}$$
### ESERCIZIO
$\begin{cases}x+2y+3z=1 \\ 2x+3y+z=3 \\ x+y+4z=2\end{cases}$            $x \begin{pmatrix}1 \\ 2 \\ 1\end{pmatrix}+y \begin{pmatrix}2 \\ 3 \\ 1\end{pmatrix}+z \begin{pmatrix}3 \\ 1 \\ 4\end{pmatrix}=\begin{pmatrix}1 \\ 3 \\ 2\end{pmatrix}$

#SOLUZIONE 

$A=\begin{pmatrix}1 & 2 & 3 \\ 2 & 3 & 1 \\ 1 & 1 & 4\end{pmatrix}$;     $\det A=12+2+6-9-1-16=-6 \implies$ il sistema è di cramer

$x= \frac{\det A_{(1)}}{\det A}=-\frac{1}{6}\det \begin{pmatrix}1 & 2 & 3 \\ 3 & 3 & 1 \\ 2 & 1 & 4\end{pmatrix}=-\frac{1}{6}(12+4+9-18-1-24)=\frac{-18}{-6}=3$

$y=\frac{\det A_{2}}{\det A}=-\frac{1}{6}\det \begin{pmatrix} 1 & 2 & 1 \\ 2 & 3 & 3 \\ 1 & 1 & 2\end{pmatrix}=-\frac{1}{6}(6+6+2-3-3-8)=-\frac{1}{6}(25-19)=-1$

$z=\frac{\det A_{3}}{\det A}=\frac{1}{6}\det \begin{pmatrix}1 & 2 & 1 \\ 2 & 3 & 3  \\ 1 & 1 & 2\end{pmatrix}=-\frac{1}{6}\det \begin{pmatrix}6+6+2-3-3-3-8\end{pmatrix}=-\frac{1}{6}(14-14)=0$
$\implies$ la  soluzione del sistema è $X=\begin{pmatrix}3 \\ -1 \\ 0\end{pmatrix}$
## ESERCIZIO

$\begin{cases}hx+hy=2 \\ 3x+hy=5\end{cases}$          $h\in R$; quando è un sistema di cramer

#SOLUZIONE 

$\begin{pmatrix}h & h \\ 3 & h\end{pmatrix}\begin{pmatrix}x \\ y\end{pmatrix}=\begin{pmatrix}2 \\ 5\end{pmatrix}$ ;

$\det A=h^2-3h=h(h-3)$ 
$\det A=0 \iff h(h-3)\iff h=0 \ \text{oppure} \ h=3$

per ogni h=0 e h=3 il sistema non è di cramer

supponiamo $h\neq 0$ e $h\neq 3$.

$x=\frac{1}{h(h-3)}\det \begin{pmatrix}2 & h \\ 5  & h\end{pmatrix}=\frac{2h-5h}{h(h-3)}=\frac{-3h}{h(h-3)}=\frac{3}{3-h}$

$y=\frac{1}{h(h-3)}\det \begin{pmatrix}h & 2 \\ 3 & 5\end{pmatrix}=\frac{5h-6}{h(h-3)}$

$\implies$ la soluzione del sistema è $X=\begin{pmatrix}\frac{3}{3-h} \\ \frac{5h-6}{h(h-3)}\end{pmatrix}$

## RANGO DI UNA MATRICE 

### DEFINIZIONE (SOTTOMATRICE)
sia  $A\in K^{m,n}.$        sia $I\subseteq \{1,\dots,m\}$  e  $J\subseteq\{1,\dots,n\}$ 
la matrice $$A_{I,J}=(a_{i,j}|\ i\in I\wedge j\in J)$$ si chiama sottomatrice di A individuata da I e J

### ESEMPIO

sia $A=\begin{pmatrix}a_{11} & a_{12} & a_{13} & a_{14} & a_{15} \\ a_{21} & a_{22} & a_{23} & a_{24}  & a_{25}  \\ a_{31}  & a_{32} & a_{33} & a_{34} & a_{35}\end{pmatrix}\in K^{3,5}$

prendiamo $I=\{1,3\},\ J=\{2,3,5\}\implies A_{I,J}=\begin{pmatrix}a_{12} & a_{13 }  & a_{15}  \\ a_{32} & a_{33} & a_{35}\end{pmatrix}\in K^{2,3}$
$A_{I,J}$ è una sottomatrice di $A$.

### DEFINIZIONE (minore di ordine r)
sia $A\in K^{m,n}$    si chiama minore di ordine r di A, il determinante di una sottomatrice quadrata di A, di ordine r (ovvero con r righe e r colonne)
### ESEMPIO

sia $A=\begin{pmatrix}1 & 2 & 3 & 4 & 5 \\ 3 & 8 & 6 & 1 & 3 \\ 5 & 1 & 9 & 2 & 4\end{pmatrix}\in R^{3,5}$ 

$I=\{1,2\}$,  $J=\{3,5\}$ $\implies$ $A_{I,J}=\begin{pmatrix}3 & 5 \\ 6 & 3\end{pmatrix};$     
$$M=\det A_{I,J}$$
## DEFINIZIONE (rango di una matrice)
sia $A\in K^{m,n}$.
si chiama ==RANGO DI A== l'ordine massimo di un minore (M) non nullo di $A$. 
## NOTAZIONE
indicheremo il rango di A con $rk (A)$
### ESEMPIO

sia $A=\begin{pmatrix}2 & 3 & 4 & 2 & 1 \\ 5 & 1 & 3 & 1 & 4 \\ 7 & 4 & 7 & 3 & 5\end{pmatrix}\in K^{3,5}$        (notiamo che $R_{3}=R_{1}+R_{2}$)

calcoliamo il rango di $A$

$M=\det \begin{pmatrix}2 & 3 \\ 5 & 1\end{pmatrix}=2-15=-13 \implies rk(A)\geq 2$
inoltre essendo $R_{3}=R_{1}+R_{2}$, tutti i minore di ordine 3 sono nulli di A sono nulli.
$rk(A)=2$

## DEFINIZIONE (matrice ridotta per righe)
sia $A\in K^{m,n}$ , A si dice ridotta per righe se in ogni riga non nulla esiste un elemento non nullo (detto pivot) al di sotto del quale vi sono solo zeri.

### ESEMPIO

sia $A=\begin{pmatrix}4 & 7 & 5 & *9* & 1 & 3 \\ 0 & 0 & 0 & 0 & 0 & 0 \\ 3 & *4* & 2 & 0 & 5 & 1 \\ 6 & 0 & 9 & 0 & 2 & *3* \\ *7* & 0 & 2 & 0 & 5 & 0\end{pmatrix}$

$A$ è ridotta per righe. 
consideriamo il minore individuato dai pivot:
$M=\det A_{\{1,3,4,5\}\{1,2,4,6\}}=\det \begin{pmatrix}4 & 7 & 9 & 3 \\ 3 & 4 & 0 & 1 \\ 6 & 0 & 0 & 3 \\ 7 & 0 & 0 & 0\end{pmatrix}=\pm \det \begin{pmatrix}9 & 7 & 3 & 4 \\ 0 & 4 & 1 & 3 \\ 0 & 0 & 3 & 6 \\ 0 & 0 & 0 & 7\end{pmatrix}\neq0$ (abbiamo spostato le colonne)

$rk(A)=4$

### PROPOSIZIONE
il rango di una matrice ridotta per righe è uguale al numero di righe non nulle.

## METODO DI RIDUZIONE
ogni matrice si può trasformare in una matrice ridotta per righe, senza alterare il rango.
una trasformazione che non altera il rango della matrice è:
$$R_{i}=R_{i}+a\cdot R_{j}, \ \text{con} \ j\neq i,  \ a\in K$$
### ESERCIZIO
$A=\begin{pmatrix}2 & 3 & 4 & 2 & 1 \\ 5 & 1 & 3 & 1 & 4 \\ 7 & 4 & 7 & 3 & 5\end{pmatrix}\in K^{3,5}$


$A  (R_{2}\equiv R_{2}-4R_{1})(R_{3}\equiv R_{3}-5R_{1})\implies \begin{pmatrix}2 &  3 & 4 & 2 & 1  \\ -3 & -11 & -13 & -7 & 0 \\ -3 & -11 & -13 & -7 & 0\end{pmatrix}$  
$(R_{3}\equiv R_{3}-R_{2})\implies \begin{pmatrix}2 & 3 & 4 & 2 & 1 \\ -3 & -11 & -13 & -7 & 0 \\ 0 & 0 & 0 & 0 & 0\end{pmatrix} \implies rk(A)=rk \begin{pmatrix}2 & 3 & 4 & 2 & *1* \\ -3 & -11 & -13 & *-7* & 0 \\ 0 & 0 & 0 & 0 & 0\end{pmatrix}$ $rk(A)=2$

### NOTAZIONE
sia $AX=B$ un sistema lineare.

sia $(A|B)$ la matrice ottenuta da $A$ affiancando la colonna B

quindi se $A\in K^{m,n}\implies(A|B)\in K^{m,n+1}$

## TEOREMA DI ROUCHE-CAPELLI
un sistema lineare $AX=B$ è risolubile $\iff$ $rk(A)=rk(A|B)$ 
### ESERCIZIO
$\begin{cases}2x+3y+5y=1 \\ x+4y+2z=3\end{cases}$

#SOLUZIONE 

$\begin{pmatrix}2 & 3 & 5 & 1 \\ 1 & 4 & 2 & 3\end{pmatrix}$;       $\det \begin{pmatrix}2 & 3 \\ 1 & 4\end{pmatrix}=8-3=5\neq 0$

$\implies rk\begin{pmatrix}2 & 3 & 5 \\ 1 & 4 & 2\end{pmatrix}=rk \begin{pmatrix}2 & 3 & 5 & 1 \\ 1 & 4 & 2 & 3\end{pmatrix}=2 \implies$ il sistema è risolubile

isoliamo $z$ dato che è la variabile libera
$\begin{cases}2x+3y=1-5z \\ x+4y=3-2z\end{cases}$

$x=\frac{1}{5}\det \begin{pmatrix}1-5z & 3 \\ 3-2z & 4\end{pmatrix}=\frac{1}{5}[4\cdot(1-5z)-3(3-2z)]=\frac{1}{5}(4-20z-9+6z)=\frac{-5-14z}{5}$

$y=\frac{1}{5}\det \begin{pmatrix}2 & 1-5z \\ 1 & 3-2z\end{pmatrix}=\frac{1}{5}[2(3-2z)-(1-5z)]=\frac{1}{5}(6-4z-1+5z)=\frac{5+z}{5}$

l'insieme delle soluzioni è $y=\{\frac{-5-14z}{5},\frac{5+z}{5},z|z\in R\}$

il sistema ha $\infty^1$ soluzioni

### NOTAZIONE
sia $AX=B$ un sistema lineare risolubile.
sia $r=rk(A)=rk(A|B)$.
sia $A\in K^{m,n}$ .
il numero di variabili libere è $n-r$ e diremo che il sistema ha $\infty^{n-r}$ soluzioni
nel caso $n=r$ il sistema ha una ed una sola soluzione

### ESERCIZIO
$\begin{cases}2x+y=5 \\ x+y=3 \\ 3x-y=h\end{cases}$ ;               $h\in R$ 

#SOLUZIONE 

$(A|B)=\begin{pmatrix}2 &  1 & 5  \\ 1 & 1 & 3 \\ 3 & -1 & h\end{pmatrix}$;    $\det (A|B)=2h+9-5-15+6-h=h-5$
$\det (A|B)=0\iff h-5=0\iff h=5$

per $h=5$ 

$A|B=\begin{pmatrix}2 & 1 & 5 \\ 1 & 1 & 3 \\ 3 & -1 & 5\end{pmatrix}\implies rk(A)=rk(A|B)=2\implies$ il sistema è risolubile.

$n=2$, $r=2$ $\implies$ $n-r=0$ $\implies$ il sistema ha una ed una sola soluzione

$\begin{cases}2x+y=5 \\ x+y=3\end{cases}\implies \begin{pmatrix}2 & 1 & 5 \\ 1 & 1 & 3\end{pmatrix}(R_{2}\equiv R_{2}-R_{1})\implies \begin{pmatrix}2 & 1 & 5 \\ -1 & 0 & -2\end{pmatrix}\implies \begin{pmatrix}2 & 1 & 5 \\ 1 & 0 & 2\end{pmatrix}$

$\begin{cases}2x+y=5 \\ x=2\end{cases}\implies \begin{cases}x=2 \\ y=1\end{cases}$            $X=\begin{pmatrix}2 \\ 1\end{pmatrix}$

# Spazi Vettoriali
ricordiamo che $(K^{m,n},+)$ è un gruppo abeliano.
e ricordiamo che anche il prodotto di uno scalare per una matrice 
$$K\times K^{m,n}\rightarrow K^{m,n}$$
### *DEFINIZIONE* (K-spazio vettoriale)
sia $(K,+,\cdot)$ un campo i cui elementi si chiamano scalari.
sia $(V,+)$ un gruppo abeliano i cui elementi sono vettori.
diremo che $V$ è un **K-spazio vettoriale** se è definito un prodotto tra uno scalare e un vettore il cui risultato è un vettore, ovvero $$K\times V \rightarrow V$$ che gode delle seguenti proprietà:
1. $(a+b)\cdot v=a\cdot v+b\cdot v$,       $\forall a,b\in K,\  \forall v\in V$
2. $a(u+v)=a\cdot u+a\cdot v$,        $\forall a\in K,   \ \ \forall u,v\in V$
3. $a(b\cdot v)=(a\cdot b)\cdot v$,               $\forall a,b\in K, \ \ \forall v\in V$
4. $1\cdot v=v$,                               $\forall v\in V$            (1 è l'unità in $K$)

#### ESEMPIO 
$V=K^{m,n}$ è uno spazio vettoriale su K
in particolare $V=K^{n}=K^{1,n}$ è un K-spazio vettoriale
#### NOTAZIONE 
sia $V$ un K-spazio vettoriale.
$(K,+,\cdot)$ è un campo, gli elementi neutri di K sono 0 e 1.
$(V,+)$ è un gruppo abeliano, l'elemento neutro di $V$ si indica $\theta$ e si chiama vettore nullo

##### LEGGE DI ANNULLAMENTO DEL PRODOTTO
sia $V$ un K-spazio vettoriale.
siano $a\in K, \ v\in V$ .
#### DIMOSTRAZIONE
supponiamo $a=0$
$$a\cdot v=\theta=(0+0)\cdot v=0\cdot v+0\cdot v \implies 0\cdot v=0\cdot v+0\cdot v\implies \theta=0\cdot v$$
supponiamo $v=\theta$ 
$$a\cdot v=a\cdot O_{-}=a(O_{-}+O_{-})=a\cdot O_{-}=a\cdot O_{-}+a\cdot O_{-}=O_{-}=a\cdot O_{-}$$
supponiamo $a\cdot v=\theta$
se $a=0$ abbiamo finito, quindi possiamo supporre $a\neq 0 \implies$ a è invertibile rispetto al prodotto in K.
sia $a^-1$ il suo inverso:
$a\cdot v=\theta \implies a^{-1}(a\cdot v)=a^{-1}\cdot \theta\implies (a^{-1}\cdot a)\cdot v=\theta\implies 1\cdot v=\theta \implies v=\theta$  
### *DEFINIZIONE*
sia V un K-spazio vettoriale.
sia $S \subseteq V$, diremo che $S$ è un sottospazio di V se S è a sua volta un K-spazio vettoriale rispetto alle stesse operazioni definite su V
![[Screenshot 2025-11-08 012327.png]]
### PROPOSIZIONE 
sia V un K-spazio vettoriale, sia $S\subseteq V$.
S è un sottospazio di V se e solo se valgono le seguenti proprietà: 
1. $\theta \in S$
2. $\forall a,b\in K, \ \forall u,v\in S \implies a\cdot u+b\cdot v\in S$            **chiusura rispetto alla combinazione lineare**
#### ESEMPIO
sia $V=R^2$,            sia $S=\{(x,y)\in R^{2}| \ x+2y=1\}\subseteq R^{2}$
$S$ non è un sottospazio, infatti $\theta = (0,0)\not\in S$.

#### ESEMPIO
sia $V=R^2$;  sia $S=\{(x,y)\in R^2|x^2-y^2=0\}\subseteq R^2$;
$\vec{u}=(1,1)\in S$,  $\vec{v}=(1,-1)\in S$ $\implies$ $\vec{v}+\vec{u}=(2,0)\not\in S$
$\implies S$ non è un sottospazio, dato che la somma non è interna ad S.
### PROPOSIZIONE
sia $A\in K^{m,n}$.  sia $S=\{X\in K^n|AX=\theta\}\subseteq K^n$.
$S$ è un sottospazio di $K^n$.
#### DIMOSTRAZIONE
1. $\theta\in S$;  $A\cdot\theta=\theta\implies\theta\in S$
2. siano $a,b\in K$; siano $a,b\in K$, siano $X,Y\in S\implies AX=\theta, \ AY=\theta$ 
  $a\cdot X + b\cdot Y\in S$?
 $$$A(aX+bY)=a(AX)+b(AY)=a\cdot\theta+b\cdot\theta=\theta\implies a\cdot X+b\cdot Y\in S$$

#### ESEMPIO 
i sottospazi di $R^2$ sono: $\{\theta=(0,0)\},\ R^2$

gli altri sottospazi di $R^2$ sono tutte le rette passanti per $\theta$

### PROPOSIZIONE 
sia $V$ un K-spazio vettoriale.
siano $U\subseteq V$ e $W\subseteq V$ sottospazi $\implies U\cap W$ è un sottospazio di $V$
#### DIMOSTRAZIONE
1. $\theta\in U$ ;  $\theta\in W \implies\theta\in U\cap W$
2. siano $a,b\in K$ ; siano $v,z\in U\cap W\implies v,z\in U$ e $v,z\in W$ ;
	$a\cdot v+b\cdot z\in U$;  $a\cdot v+b\cdot z\in W \implies a\cdot v+b\cdot z\in U\cap W$ ;

### *DEFINIZIONE* (SOMMA DI SOTTOSPAZI)
sia $V$ un K-spazio vettoriale.
siano $U\subseteq V$ e $W\subseteq V$ sottospazi.
poniamo $$U+W=\{u+w \ |\ u\in U, w\in W\}$$
![[Schermata del 2025-11-17 18-27-28.png]]

$U+W$ si chiama *somma* dei sottospazi $U$ e $W$

### PROPOSIZIONE
la somma di sottospazi è un sottospazio.
#### DIMOSTRAZIONE
1. $\theta \in U$, $\theta\in W \implies$ $\theta=\theta+\theta\in U+W$
2. siano $a,b\in K$ ; siano $v_{1}\in U+W$ e $v_{2}\in U+W$ ;
	$v_{1}\in U+W \implies v_{1}=u_{1}+w_{1}$ con $u_{1}\in U$ e $w_{1}\in U+W$
	$v_{2}\in U+W\implies v_{2}=u_{2}+w_{2}$ con $u_{2}\in U$ e $w_{2}$
	$$av_{1}+bv_{2}=a(u_{1}+w_{1})+b(u_{2}+w_{2})=au_{1}+aw_{1}+bu_{2}+bw_{2}=(au_{1}+bu_{2})+(aw_{1}+bw_{2})$$
	$$\implies av_{1}+bv_{2}\in U+W$$
### *DEFINIZIONE* (Combinazione Lineare Vettoriale)
sia $V$ un K-spazio vettoriale.
siano $a_{1},\dots,a_{n}\in K$, siano $v_{1},\dots,v_{n}\in V$.
il vettore $a_{1}v_{1}+\dots,a_{n}v_{n}$ si chiama *combinazione lineare dei vettori*  $v_{1},\dots,v_{n}$
$$\sum_{i=1}^{n}a_{i}v_{i}$$
#### NOTAZIONE 
sia $V$ un K-spazio vettoriale.
sia $S\subseteq V$.
poniamo $\mathcal{L}(S)=\{\text{tutte le possibile combinazioni lineari di vettori in S}\}$

### PROPOSIZIONE
sia $V$ un K-spazio vettoriale. sia $S\subseteq V$, $S\neq \theta\implies\mathcal L(S)$ è un sottospazio di V

### *DEFINIZIONE* (INSIEME DI GENERATORI)
$S$ si chiama *insieme di generatori* di $\mathcal L(S)$ ed $\mathcal L(S)$ si chiama *sottospazio generato* da S.
#### ESEMPIO 
sia $V$ un K-spazio vettoriale.
sia $S=\{v\}\implies\mathcal L(S)=\{av\ | \ a\in K\}$
sia $S=\{u,v\}\implies\mathcal L(S)=\{au+bv \ |\ a,b\in K\}$
#### ESEMPIO 
sia $V=R^3$. siano $u=(1,1,0)$ $v=(0,1,1)$
$S=\{u,v\}$; $\mathcal L(S)=\{au+bv | a,b\in R\}$=$\{a(1,1,0)+b(0,1,1)\ |a,b\in R\}=\{(a,a+b,b)\ | a,b\in R\}$
$\begin{cases}x=a \\ y=a+b \\ z=b\end{cases}\implies y=x+z\implies x-y+z=0\implies\mathcal L(S)=\{(x,y,z)\in R^{3}|x-y+z=0 \}$
#### ESEMPIO 
sia $A=\begin{pmatrix}1 & 2 & 3 \\ 4 & 5 & 6\end{pmatrix}\in R^{2,3}$
sia $W=\{(x,y,z)\in R^{3}|\begin{pmatrix}1 & 2 & 3 \\ 4 & 5 & 6\end{pmatrix}\begin{pmatrix}x \\ y \\ z\end{pmatrix}=\theta\}$ è un sottospazio di $R^3$
![[Schermata del 2025-11-17 19-16-16.png]]

# LEZIONE 8

### OSSERVAZIONE
sia V un K-spazio vettoriale, ovviamente $V=\mathcal L(V)$.
quindi ogni spazio vettoriale ha insieme di generatori.
### *DEFINIZIONE*
un K-spazio vettoriale V si dice *finitamente generato* se $\exists S\subseteq V$, S finito, tale che $V=\mathcal L(S)$.
#### ESEMPIO
$V=K^3$ è finitamente generato.
infatti sia $S=\{(1,0,0),(0,1,0),(0,0,1)\}\implies K^{3} =\mathcal L(S)$
infatti sia $(x,y,z)\in K^{3}\implies(x,y,z)=xl_{1}+yl_{2}+zl_{3}$, cioè $(x,y,z)$ è combinazione lineare di $l_{1},l_{2},l_{3}$ 
#### ESEMPIO 
più in generale, sia $V=K^{m,n}$.
sia $E_{i,j}\in K^{m,n}$ la matrice che ha $1$ nel posto $(i,j)$ e $0$ altrove.
sia $$\mathcal L=\{E_{i,j}|1\leq j \leq n\}$$
$\mathcal E$ genera $K^{m,n}\implies K^{m,n}$ è finitamente generato
### *DEFINIZIONE*
sia V un K-spazio vettoriale.
siano $v_{1},\dots,v_{n}\in V$.
diremo che $v_{1},\dots,v_{n}$ sono *linearmente dipendenti* se esistono n scalari $a_{1},\dots,a_{n}\in K$, non tutti nulli, tali che $$a_{1}v_{1}+\dots+a_{n}v_{n}=\theta$$
altrimenti si diranno *linearmente indipendenti*.
#### ESEMPIO
siano $v_{1}=(1,2,3),v_{2}=(3,2,1),v_{3}=(1,1,1)$;
$v_{1}+v_{2}=(4,4,4)=4v_{3}\implies 1v_{1}+1v_{2}-4v_{3}=\theta \implies v_{1},v_{2},v_{3}$ sono linearmente dipendenti
### CRITERIO DI INDIPENDENZA LINEARE 
sia V un K-spazio vettoriale.
$v_{1},\dots,v_{n}\in V$ sono linearmente indipendenti se e solo se:
1. $v_{1}\neq \theta$
2. $v_{i}\in\mathcal L(v_{1},\dots,v_{i-1}),$ per $2\leq i \leq n$
##### ESERCIZIO
dire se i vettori $v_{1}=(1,1,0), v_{2}=(0,1,1),v_{3}=(1,2,3)$ sono linearmente indipendenti.
### *DEFINIZIONE* 
sia V un K-spazio vettoriale.  sia $\mathcal L\subseteq V$, $\mathcal L$ finito.
$\mathcal L$ si dice insieme libero se i vettori in $\mathcal L$ sono linearmente indipendenti.
sia $\mathcal B\subseteq V$.
diremo che $\mathcal B$ è una base di V se $\mathcal B$ è un insieme libero di generatori di V.
### METODO DEGLI SCARTI SUCCESSIVI
sia V un K-sp. vett. finitamente generato.
sia $\mathcal G\subseteq V$ un insieme finito di generatori di V (quindi $V=\mathcal L(G)$)
$\implies$ esiste una base $\mathcal B$ di V, $\mathcal B\subseteq G$.
#### DIMOSTRAZIONE 
sia $\mathcal G=\{v_{1},\dots,v_{s}\}$

$v_{1}=\theta$ *lo scartiamo*
$v_{1}\neq \theta$ lo lasciamo

se abbiamo scartato $v_{1}$, ripetiamo su $v_{2}$ la procedura.
se $v_{1}\neq \theta$

$v_{2}=v_{2}\in \mathcal L(v_{1})$ *lo scartiamo*
$v_{2}=v_{2}\not\in \mathcal L(v_{1})$ lo lasciamo

continuando con questa procedura alla fine otteniamo un insieme di vettori 
$$\mathcal B=\{u_{1},\dots,u_{r}\}\subseteq\mathcal G$$
$\mathcal B$ è una base di V.
### ESTENSIONE DI UN INSIEME LIBERO AD UNA BASE
sia V un K-sp. vett., finitamente generato.
sia $L\subseteq V$ un insieme libero (finito) $\implies$ $\exists$ una base $\mathcal B$ di V tale che $\mathcal L\subseteq B$.
#### DIMOSTRAZIONE
sia $$L=\{u_{1},\dots,u_{r}\}$$ un insieme libero.
sia $G=\{v_{1},\dots,v_{s}\}$ un insieme finito di generatori di V.
consideriamo la "lista" di vettori: $u_{1},\dots,u_{r},v_{1},\dots,v_{s}$
a questa lista applichiamo il metodo degli scarti successivi.
nessuno degli $u_{i}$ si potrà scartare $\implies$ alla fine otterremo una base $\mathcal B$ tale che $\mathcal L \subseteq \mathcal B$.
##### ESERCIZIO
siano $v_{1}=(2,1,0)$, $v_{2}=(1,1,0)$ in $\mathbb R^3$
1. provare che $L=\{v_{1},v_{2}\}$ è un insieme libero.
2. estendere $L$ ad una base di $\mathbb R^3$

### LEMMA DI STEINITZ
sia V un K-sp. vett., finitamente generato.
sia $\mathcal G\subseteq V$ un insieme finito di generatori; 
sia $L\subseteq V$ un insieme libero $\implies$
$$|L|\leq|G|$$
($|S|$ numero di elementi in S)

### COROLLARIO
sia V un K-sp. vett. fin. gen.
siano $\mathcal B_{1}$ e $\mathcal B_{2}$ due basi di V $\implies |\mathcal B_{1}|=|\mathcal B_{2}|$

#### DIMOSTRAZIONE

$\mathcal B_{1}$ è libero
$\mathcal B_{2}$ è insieme di generatori
$\downarrow$
$|\mathcal B_{1}|\leq|\mathcal B_{2}|$
		$\implies$ $|\mathcal B_{1}|=|\mathcal B_{2}|$
$|\mathcal B_{2}|\leq|\mathcal B_{1}|$
$\uparrow$
$\mathcal B_{2}$ è libero
$\mathcal B_{1}$ è insieme di generatori

### DEFINIZIONE
sia V un K-sp. vett. fin. gen. 
si chiama *dimensione di V* il numero di elementi di una base di V.
la indichiamo con $dim_{k}V$ 
#### ESEMPIO
sia $V=K^{m,n}$.    $\mathcal L=\{E_{i,j}|\ 1\leq i\leq m, \ 1 \leq j\leq n\}$ è una base di $K^{m,n}$, detta *base canonica*
$\implies dim_{k}K^{m,n}=\mathcal L=m\cdot n$. 
### FORMULA DI GRASSMANN
sia V un K-sp. vett. fin. gen. e siano $U,W\subseteq$ sottospazio
$\implies dim_{k}(U+W)=dim_{k}U+dim_{k}W-dim_{k}(U\cap W)$
### PROPOSIZIONE
sia V un K-sp. vett. fin. gen.
sia $W\subseteq V$ un sottosp.
1. $dim_{k}W\leq dim_{k}V$
2. $dim_{k}W = dim_{k}V \iff W=V$
#### DIMOSTRAZIONE
1. sia $\mathcal B_{W}$ una base di W $\implies \mathcal B_{W}$ è un insieme libero in V
$\implies$   $\mathcal B_{W}$ si può estendere ad un base $\mathcal B_{V}$ di V 
$\implies$ $\mathcal B_{W}\subseteq\mathcal B_{V} \implies |\mathcal B_{W}|\leq|\mathcal B_{V}|\implies dim_{k}W\leq dim_{k}V$
2.  supponiamo che $dim_{k}W=dim_{k}V.$  siano $\mathcal B_{W}\subseteq \mathcal B_{V}, \mathcal B_{W}$ base di W e $\mathcal B_{V}$ base di V.
   $|\mathcal B_{W}|=|\mathcal B_{V}|\implies \mathcal B_{W}=\mathcal B_{V}\implies\mathcal L(\mathcal B_{W})=\mathcal L(\mathcal B_{V})\implies W=V$ 

viceversa, se $W=V \implies dim_{k}W=dim_{k}V$
### DEFINIZIONE
sia $A\in K^{m,n}. \implies A=\begin{pmatrix}R_{1} \\ \dots \\R_{m}\end{pmatrix}=(C_{1},\dots,C_{n})$

$R_{i}\in K^n$ riga di A, $C_{j}\in K^m$ colonna di A.

si chiama *spazio delle righe di A*, il sottospazio $\mathcal L_{R}(A)=\mathcal L(R_{1},\dots,R_{m})$
si chiama *spazio delle colonne di A*, il sottospazio $\mathcal L_{C}(A)=\mathcal L(C_{1},\dots,C_{n})$

#### ESEMPIO
sia $A=\begin{pmatrix}1 & 2 & 3 \\ 4 & 5 & 6\end{pmatrix}\in R^{2,3}$
$\mathcal L_{c}(A)=\mathcal L((1,4),(2,5),(3,6))\subseteq R^2$;  $\mathcal L_{r}(A)=\mathcal L((1,2,3),(4,5,6))\subseteq R^3$

### TEOREMA DI KRONECKER
sia $A\in K^{m,n}\implies dim_{k}\mathcal L_{r}(A)=dim_{k}\mathcal L_{c}(A)=rk A$
![[Schermata del 2025-11-17 23-04-34.png]]
### TEOREMA DI ROUCHÉ-CAPELLI
sia $AX=B$ un sistema lineare. esso è risolubile $\iff rkA=rk(A|B)$
#### DIMOSTRAZIONE
![[Schermata del 2025-11-17 23-06-48.png]]
### PROPOSIZIONE
sia $A\in K^{m,n}$.
sia $W=\{X\in K^{n}|AX=0\}\subseteq K^n$.
sappiamo che W è un sottospazio di $K^n$.
$$dim_{k}W=n-rkA$$
#### ESEMPIO
![[Schermata del 2025-11-17 23-09-27-1.png]]

### PROPOSIZIONE
sia $A\in K^{n-1,n}$, con $rkA=n-1$
sia $W=\{X\in K^{n}|AX=0\}$
1. $dim_{k}W=n-(n-1)=1$
2. una base di W è il vettore le cui componenti sono i minori a segno alterno di A.

# LEZIONE 9
### *DEFINIZIONE*
sia $A\in K^{m,n}$, sia M un minore di A di ordine r.
si chiama orlato di M un minore di ordine r+1, contenente M.
### TEOREMA
sia $A\in K^{m,n}$, $rkA=r$ se e solo se:
1. A contiene un minore M, di ordine r, non nullo
2. tutti gli orlati di M sono nulli.
# Applicazioni Lineari
# LEZIONE 10
### DEFINIZIONE
siano U e V K-spazi vettoriali.
sia $U\to V$ una funzione.
diremo che $\mathcal f$ è un'applicazione lineare se:$$f(a_{1}u_{1}+a_{2}u_{2})=a_{1}f(u_{1})+a_{2}f(u_{2}), \ \forall a_{1},a_{2}\in K; \ \forall u_{1},u_{2}\in U$$
#### ESEMPIO
sia $A\in K^{m,n}$.
allora A definisce una funzione $K^n\to K^m$, $f_{A}(X)=AX\in K^m$

$F_{A}$ è un applicazione lineare, infatti:
siano $b_{1},b_{2}\in K,\ x_{1},x_{2}\in K^n$
$f_{A}(b_{1}X_{1}+b_{2}X_{2})=A(b_{1}X_{1}+b_{2}X_{2})=A(b_{1}X_{1})+A(b_{2}X_{2})=b_{1}(AX_{1})+b_{2}(AX_{2})=b_{1}f_{A}(X_{1})+b_{2}f_{A}(X_{2})$
#### ESEMPIO
sia $A=\begin{pmatrix}1 & 2 & 3 \\ 4 & 5 & 6\end{pmatrix}\in \mathbb R^{2,3}\implies A$ definisce un applicazione lineare $\mathbb R^{3}\to\mathbb R^2$ .
vediamo come $F_{A}$ agisce sui vettori della base canonica di $\mathbb R^3$, $\mathcal E$ .

$\mathcal E=\{l_{1},l_{2},l_{3}\}$ con $l_{1}=(1,0,0), \ l_{2}=(0,1,0), \ l_{3}=(0,0,1)$
$F_{A}(l_{1})=\begin{pmatrix}1 & 2 & 3  \\  4 & 5 & 6\end{pmatrix}\begin{pmatrix}1 \\ 0 \\ 0\end{pmatrix}=\begin{pmatrix}1 \\ 2\end{pmatrix}=C_{1}$
$F_{A}(l_{2})=\begin{pmatrix}1 & 2 & 3 \\ 4 & 5 & 6\end{pmatrix}\begin{pmatrix}0 \\ 1 \\ 0\end{pmatrix}=\begin{pmatrix}2 \\ 4\end{pmatrix}=C_{2}$
$F_{A}(l_{3})=\begin{pmatrix}1 & 2 & 3 \\ 4 & 5 & 6\end{pmatrix}\begin{pmatrix}0 \\ 0 \\ 1\end{pmatrix}=\begin{pmatrix}3 \\ 6\end{pmatrix}=C_{3}$

### PROPOSIZIONE
sia $U\to V$ un applicazione lineare.
![[Schermata del 2025-11-18 17-05-48.png]]
#### DIMOSTRAZIONE
$f(\theta_{U})=f(\theta_{U}+\theta_{U})=f(\theta_{U})+f(\theta_{U})$
$\implies f(\theta_{U})=f(\theta_{U})+f(\theta_{U})\implies\theta_{V}=f(\theta_{U})$

### IMMAGINE E CONTROIMMAGINE
siano $A$ e $B$ due insiemi, e sia $A\to B$ una funzione.
![[Schermata del 2025-11-18 17-15-34.png]]
sia $X\subseteq A$.
si chiama *immagine di X*, l'insieme:
$$f(X)=\{f(x)|\ x\in X\}$$
in particolare se $X=A$, poniamo $\mathcal {Im}f=f(A)$, detta *immagine* di $f$
ricordiamo inoltre che $f$ si dice suriettiva se $\mathcal Imf=B$.
![[Schermata del 2025-11-18 18-41-29.png]]
sia $Y\subseteq B$.
si chiama *controimmagine* di Y, l'insieme:
$$f^-1=\{a\in A|\ f(a)\in Y\}$$
#### ESEMPIO
sia $\mathbb R\to \mathbb R, \ \ f(x)=x^3-x$
sia $Y=\{0\}$   $f^-1(\{0\})=\{x\in \mathbb R| \ f(x)\in \{0\}\}=\{x\in\mathbb R| \ x^3-x=0\}$;
$x^{3}-x=0\iff x(x^{2}-1)=0\iff x=0,1,-1$
$\implies f^-1(\{0\})=\{-1,0,1\}$
sia $Z=[0,+\infty[\subseteq \mathbb R$
$f^-1(Z)=\{x\in\mathbb R |\ f(x)\in[0,+\infty[\ \}=\{x\in\mathbb R |x^3-x\in[0,+\infty[\ \}=\{x\in\mathbb R|\ x^{3}-x\geq 0\}=[-1,0]\cup[1,+\infty[$

$x^{3}-x\geq 0$       $x(x^{2}-1)\geq 0$
![[Schermata del 2025-11-18 18-53-35.png]]

### PROPOSIZIONE
sia $U\to V$ un applicazione lineare.
1. sia $W\subseteq U$ un sottospazio $\implies$ $f(W)$ è un sottospazio di V
2. sia $Z\subseteq V$ un sottospazio $\implies$ $f^{-1}(Z)$ è un sottospazio di U

#### DIMOSTRAZIONE

1. $\theta_{V}\in f(W)$? poiché W è un sottospazio di U, $\theta_{U}\in W\implies\theta_{V}=f(\theta_{U})\in f(W)$
	resta da dimostrare che $f(W)$ è chiuso rispetto alle combinazioni lineari
siano $a,b\in K$, siano 1$v_{1},v_{2}\in f(W)\implies v_{1}=f(W_{1}),v_{2}=f(W_{2})$
$av_{1}+bv_{2}=af(W_{1})+{(W_{2}})=f(aw_{1}+bw_{2})\in f(W)$.

2. $\theta_{U}\in f^-1(Z)?$ 
	$f(\theta_{U})=\theta_{V}\in Z$, perché Z è un sottospazio di V.
	siano $a,b\in K$
