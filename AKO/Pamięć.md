
Pamięć to jest de facto *wektor liczb*.
Jeśli komórkę tworzy 8 bitów, pamięć ma *organizację bajtową*.
Dane zapisane w pamięci są nierozróżnialne od instrukcji!

W organizacji **bajtowej** 8 bitów = 1 bajt.
>16 bitów to słowo (WORD)
>32 bity (4 bajty) to słowo podwójne (DWORD)

*Bajt* zajmuje jedną komórkę danych w pamięci. Każdy bajt ma unikalny adres w *Przestrzeni adresowej*.
Przestrzeń adresowa to zbiór wszystkich liczb które stanowią adresy istniejących komórek w pamięci. Zazwyczaj przestrzeń adresowa ma liczność równą największej możliwej wartości słowa.
> Na przykład w organizacji 4-bitowej przestrzeń adresowa leży między `00` a `FF`
# Znaczność bitów
\[==M==SB __ __ __ ... __ ==L==SB]
## MSB
==Most== Significant Bit
## LSB
==Least== Significant Bit

>[!warning]
>W pamięci **zawsze** *coś* jest!

^0d8c33

>[!warning]
>Różne programy różnie wizualizują przestrzeń adresową. Zwróć uwagę czy adresy z góry na dół rosną czy maleją.
>Dodatkowo [[Stos]] rośnie odwrotnie do [[Sterta]].
