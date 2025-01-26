Równanie zwyczajne (jendocząstkowe) n-tego rzędu ma postać
F(x, y, y', ... y<sup>(n)</sup>) = q(x)
	jeśli q(x) = 0, równanie jest *jednorodne*

## Równanie o zmiennych rozdzielonych
dy/dx = g(x)h(y)
1/h(y)dy = g(x)dx ... i całkujemy
## Czynnik całkujący
1. doprowadzamy do postaci $y' + p(x)·y = q(x)$
2. ... szukamy funkcji u takiej, że $(uy)'  =  u(y' + p(x)·y)$
	u jest *czynnikiem całkującym*
	$u = e^{\int{p(x)dx}}$
3. mnożymy obie strony równania razy u
4. kolapsujemy stronę z y-em do (uy)'
5. rozwiązujemy dla y' algebraicznie i całkujemy zmienne rozdzielone
## Równanie liniowe
> W postaci $y'' + a(x)y' + b(x)y = f(x)$

Kluczem jest znaleźć *całkę ogólną równania jednorodnego* CORJ i dowolną *szczególną niejednorodnego* CSRN. CORJ + CSRN = CORN
### Metoda uzmienniania stałych