Sumę ciągu znajdujemy dla szeregów zbieżnych:
$\lim_{n \to \infty}{S_n = \lim_{n \to \infty} \sum_{k=1}^{n}(ak)}$ (ciąg sum jest zbieżny)
## Szeregi specjalne
**Szereg geometryczny:** zbieżny jeżeli q jest w (-1, 1)
	$S_\infty = \frac{1}{1-q}$
**Szereg harmoniczny:** 
	1/1 + 1/2 + 1/3 + 1/4 + ...
	jest **rozbieżny**
**Szereg Dirichleta:**
	1/1^p + 1/2^p + 1/3^p + ...
	zbieżny dla p > 1
# Badanie zbieżności szeregu
>[!info] Warunek konieczny zbieżności:
>Elementy szeregu zbieżnego muszą dążyć do 0 w nieskończoności

**Kryterium d'Alemberta:** (używać przy n!, n^n, b^n)
	r = lim an+1/an
	r > 1 => rozbieżny
	r < 1 => zbieżny
	r = 1 => nie rozstrzyga
**Kryterium Cauchy'ego:** (używać przy b^n)
	g = lim $\sqrt[n]{a_n}$
	g > 1 => rozbieżny
	g < 1 => zbieżny
	g = 1 => nie rozstrzyga
**Kryterium porównawcze pierwsze:** (o policjancie, podłodze i pijaku)
	jeżeli od pewnej N szeregi zachowują się:
	0 < bn <= an
	to jeżeli an jest zbieżny, to bn też
	a jeśli bn jest rozbieżny, to an też
**Kryterium porównawcze drugie:**
	L = lim an/bn
	L jest niezerowe => szeregi zachowują się tak samo
	L = 0 => an jest zbieżny gdy bn jest zbieżny
	L = inf => an jest rozbieżny gdy bn jest rozbieżny
>[!tip] Porównawcze drugie
>Badamy szereg $S$
>znajdujemy *zbieżny* szereg $S_2$
>$$\lim_{n \to \infty} \frac{S}{S_2} \in \mathbb{R}^{+} \implies S \text{ zbiezny}$$
>>[!tip] Jak znaleźć $S_2$?
>>$$S = \Sigma \frac{n^a + ...}{n^b + ...}$$
>>$$S_2 := \Sigma n^{\frac{b}{a}}$$

>[!Tip] Szeregi naprzemienne
>$\Sigma |(-1)^n s(n)| \text{ zbiezny} \implies \Sigma (-1)^n s(n) \text{ zbiezny}$

**Kryterium całkowe:**
	jeżeli f jest nieujemna nierosnąca w znaczącym przedziale
	oraz ak = f(k) =>
	szereg od m do inf oraz całka z f od m do inf zachowują się tak samo
### Dla szeregów naprzemiennych:
an = (-1)^n · bn
**Kryterium Leibniza:**
	lim bn = 0   oraz   bn+1 w (0, bn]   =>   zbieżny
	rozbieżności nie rozstrzyga
jeśli |an| wciąż jest zbieżny, an jest zbieżny *bezwzględnie*
w przeciwnym wypadku jest zbieżny *warunkowo*

>[!tip] Pierwszeństwo stosowania kryteriów
>1. warunek konieczny
>2. szeregi specjalne
>3. n!, n^n, b^n w wyrazach- d'Alembert
>4. a^n w szeregu - Cauchy
>5. funkcja wymierna w wyrazach - kryteria porównawcze
>6. wyrazy całkowalne - kryterium całkowe
## Przedział zbieżności
Przedział w (x0 - R, x0 + R) w którym szereg z niewiadomą x jest zbieżny.

g = lim $\sqrt{|cn|}$ = lim $|\frac{c_{n+1}}{c_n}|$

g = inf => R = 0
g = 0 => R = inf
normalnie R = 1/g
