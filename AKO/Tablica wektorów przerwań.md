---
aliases:
  - Tablica deskryptorów przerwań
---
System operacyjny eksponuje pewne funkcje dostępne na poziomie asemblera. Adresy wywołań tych funkcji znajdują się w **tablicy deskryptorów**.
Dzięki tablicy na różnych wersjach tego samego systemu operacyjnego można odwoływać się do funkcji systemowych zajmujących stałe miejsce w indeksie, zamiast do potencjalnie różnych adresów skoków.

[[AKO_2024_cz_3.pdf#page=57]]

Przerwania obsługujemy stosując [[Tryb rzeczywisty]].