---
aliases:
  - Cache
---
> [[AKO_2024_cz_5.pdf#page=30]]



# Budowa pamięci cache

Pamięć cache jest podzielona na:
- Linie
- Bloki


## Odwzorowanie bezpośrednie
Jeżeli dany blok pamięci znajduje się w cache'u, to trafia zawsze w to samo miejsce.


## Synchronizacja z pamięcią operacyjną
### Write-through
Zapis do pamięci cache jest natychmiast odwzorowywany w RAM-ie
### Write-back
Pamięć RAM jest oznaczona jako nieaktualna *bitem stanu*.

---


# Odwzorowanie asocjacyjne
Używane przez RAM przy znajdowaniu komórek [[Pamięć fizyczna|pamięci fizycznej]].
## Etykiety
	 22bit _______|___ 10bit
Na 22 bitach zapamiętujemy *etykietę* bloku, na 10 bitach offset w ramach bloku.
W pamięci [[#Cache]] trzymamy bloki.

# Odwzorowanie wielokanałowe