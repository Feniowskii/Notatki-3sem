## Zbiory liczbowe: 
- N - naturalne
- Z - całkowite
- Q - wymierne (p/q gdzie p należy do Z i q do N)
- IQ - niewymierne (R - Q)
- R - rzeczywiste (Q + IQ)
- C - zespolone (a + bi, a,b należą do R)
## Wzory skróconego mnożenia
(x +- y) = x2 +- 2xy + y2
x2 - y2 = (x+y)(x-y)
x3 +- y3 = (x +- y) (x2 -+ xy + y2) `?!`

(a + b)<sup>n</sup> - trójkąt Pascala
nCr = n!/r!\*(n-r)!
## Logarytmy
a = log<sub>b</sub> c <=> b^a = c
logarytm o podstawie b z c to taka liczba a do której trzeba podnieść b by uzyskać c
### Własności logarytmów
log 1 = 0
log_a a = 1
log_a a^y = y
a<sup>log<sub>a</sub>x</sup> = x
### Działania na logarytmach
log (xy) = log x + log y
log x^r = r log x
log_a x = log_b x / log_b a
log_a b = 1 / log_b a

---
# Funkcje
Funkcja jest parzysta gdy f(x) =  f(-x)
n.parzysta gdy f(x) = -f(-x)
Funkcja jest okresowa gdy istnieje taki okres T że f(x) = f(x+T)
	najmniejszy okres T nazywamy *podstawowym*
## Transformacje funkcji
f(x) + d : translacja o d w górę
f(x+d) : translacja o d w *lewo(!)*
cf(x) : rozciągnięcie c-krotne pionowo
f(cx) : *skurczenie(!)* c-krotne poziomo
f(-x) : obrót poziomo
-f(x) : obrót pionowo
f(|x|) : prawa strona odbita
|f(x)| : dół wywleczony
## Złożenia funkcji
D_f(g(x)) = {x takie że x jest w Dg oraz g(x) jest w Df}
## Funkcja odwrotna
Powstaje przez odbicie względem ukosu y=x
f(x) = y <=> f<sup>-1</sup>(y) = x

---
# Trygonometria
```
   /|
c / |
 /  | a
/x__|
   b
```
sin x = a/c <=> r sin = y 
cos x = b/c <=> r cos = x 
tan x = a/b <=> tan = y/x
## Tożsamości
tan x = sinx/cosx
cot x = 1/tanx ()
sin2 x + cos2 x = 1 (jedynka trygonometryczna)
`!!!`
$\sin (2x) = 2\sin x\cos x$
$\cos(2x) = \cos^2 x - \sin^2 x$
$\sin(a\pm b) = \sin a\cos b \pm \cos a\sin b$
$\cos(a\pm b) = \cos a \cos b \mp \sin a \sin b$

>METODA: równania/nierówności
>	definicja: $\arccos x = a \iff \cos a = x$
>	monotoniczność: 
>	$\cot^{-1} a > \cot^{-1} b$ (arccot jest malejący) $\iff  a < b$

# Ciągi
|             | arytmetyczny |         geometryczny         |
| :---------- | :----------: | :--------------------------: |
| suma do n   |  n(a1+an)/2  | a1 · (1-q<sup>n</sup>)/(1-q) |
| suma do inf |      -       |         a1 · 1/(1-q)         |
rosnący gdy an < an+1
nierosnący gdy an >= an+1
# Limity
lim<sub>n->inf</sub> (1 + 1/n)<sup>n</sup> = e (definicja e)