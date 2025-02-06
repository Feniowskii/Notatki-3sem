

![[AM_03_RachunekCalkowy.pdf#page=36]]

# Całki elementarne
$\int a^x dx = a^x \cdot \frac{1}{\ln a}$
![[Pochodne#Pochodne elementarne]]
# Całki niewłaściwe
$\int_a^b f(x)dx$ gdzie $f$ jest nieciągła w $a$ lub $b$, albo $a$ lub $b = \infty$
>[!tip] Zastosuj limit
>$\lim_{T \to x_0} \int_a^{x_0}f(x)dx$ gdzie $x_0$ to punkt nieciągłości.
 
>[!tip] Pierwiastki
>Użyj podstawienia $x = u^\text{wspólna wielokrotność}$
>>[!warning] To jest podstawienie za x!

%% zamiana granic całkowania a -> g(a) %%
int f'/f = ln|f| + C
int f(ax+b) = 1/a f(ax+b) + C
# Podstawienia trygonometryczne
>[!tip] iloczyn sin/cos
>sinus do potęgi nieparzystej -> podstaw $u = \cos x$, i *vice versa*
>oba do potęgi parzystej -> podstaw $u = \tan x$ ^[[[AM_03_RachunekCalkowy.pdf#page=116]]]
>>wtedy $x = \arctan u$
>>$\sin x = \frac{u}{\sqrt{1+u^2}}$ 
>>$\cos x = \frac{1}{\sqrt{1+u^2}}$
>
>[[AM_03_RachunekCalkowy.pdf#page=118|Podstawienie uniwersalne]]

# Zastosowania
## Wartość średnia
$$\frac{1}{a-b} \int_a^b f(x) dx$$

## Objętości
### Metoda dysków
### Metoda walców