[[Pamięć]]
[[Endian]]



# Komunikacja pamięć-procesor

# Budowa fizyczna
![[AKO_2024_cz_5.pdf#page=6]]
- DRAM
- SRAM
## Układ odświeżania pamięci

## Cykl dostępu do pamięci
1. Sygnał RAS (Row Address Strobe)
Wysyłany do RAMu po tym, jak magistrala adresowa ustabilizowała bity, gotowa do odczytu **rzędu**.
2. Sygnał CAS (Column Address Strobe)
Analogicznie, gotowa do odczytu **kolumny**.
3. Wysył na magistralę danych

![[AKO_2024_cz_5.pdf#page=12]]

>[!info] Zużycie energii
>$$E = V^2 \cdot f$$
>Zwiększając napięcie znacznie rośnie zużycie energii, a za tym temperatura komponentów. Ogranicza to możliwości pamięci.

# Lokalność pamięci
## Lokalność czasowa
Częste, szybkie odwołania do tych samych komórek
## Lokalność przestrzenna
Podobne adresy

![[AKO_2024_cz_5.pdf#page=28]] 
 >[!note] Slajd niekompletny o procesory wielordzeniowe
 
	 22bit _______|___ 10bit
Na 22 bitach zapamiętujemy *etykietę* bloku, na 10 bitach offset w ramach bloku [[AKO_2024_cz_5.pdf#page=34]]

![[AKO_2024_cz_5.pdf#page=33]]