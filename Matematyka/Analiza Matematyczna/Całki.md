
>[!tldr]- Definicja całki Riemanna
> ![[AM_03_RachunekCalkowy.pdf#page=36]]

# Całki elementarne
$\int a^x dx = a^x \cdot \frac{1}{\ln a}$
![[Pochodne#Pochodne elementarne]]
# Całki niewłaściwe
$\int_a^b f(x)dx$ gdzie $f$ jest nieciągła między $a$ i $b$, albo $a$ lub $b = \infty$

>[!tip] Zastosuj limit
>$\lim_{T \to x_0} \int_a^{x_0}f(x)dx$ gdzie $x_0$ to punkt nieciągłości.


int f'/f = ln|f| + C
int f(ax+b) = 1/a f(ax+b) + C
# Całkowanie przez podstawienie
>[!warning] zamiana granic całkowania
>$$\int_a^b ... \space dx$$
>$$u = g(x)$$
>$$\int_{u(a)}^{u(b)} ... \space du$$

## Pierwiastki
Użyj podstawienia $x = u^\text{wspólna wielokrotność}$
## Podstawienia trygonometryczne
- sinus do potęgi nieparzystej -> podstaw $u = \cos x$, i *vice versa*
- oba do potęgi parzystej -> podstaw $u = \tan x$ ^[[[AM_03_RachunekCalkowy.pdf#page=116]]]
>$x = \arctan u$
>$dx = \frac{1}{1+u^2}$
>$\sin x = \frac{u}{\sqrt{1+u^2}}$ 
>$\cos x = \frac{1}{\sqrt{1+u^2}}$
- Ostatecznie [[AM_03_RachunekCalkowy.pdf#page=118|Podstawienie uniwersalne]]
> $x = \arctan u/2$
- $dx = \frac{2}{1+u^2}$
> $\sin x = \frac{2u}{1+u^2}$
> $\cos x = \frac{1-u^2}{1+u^2}$

Potem rozwiąż [[#Całkowanie funkcji wymiernych]].
# Całkowanie przez części
# Całkowanie funkcji wymiernych
## Rozkład na ułamki proste
$$\frac{...}{(ax+b)(ax^2+bx+c)} = \frac{C}{ax+b} + \frac{Ax+B}{(ax^2+bx+c)} $$
$$\frac{...}{(ax+b)^2} = \frac{A}{ax+b}+\frac{B}{(ax+b)^2}$$
---
$$\frac{1}{ax^2+bx+c} = \frac{1}{(x+\alpha)^2+\beta}$$
$u = x+\alpha$
![[Pochodne#^83369c]]

$\alpha$ znajdziesz dodając i odejmując wartość $\frac{1}{a} \cdot (\frac{b}{2})^2$ (uzupełnianie kwadratu)

# Zastosowania
## Wartość średnia
$$\frac{1}{a-b} \int_a^b f(x) \space dx$$
## Długość funkcji
$$\int_a^b \sqrt{1-f'(x)^2} \space dx$$

## Pola obszaru
## Objętości
### Metoda dysków
### Metoda walców