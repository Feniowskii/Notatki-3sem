# Obsługa przerwania
>[!Tip] Nie przerywa wykonania rozkazu kiedy ma ustawioną [[Flagi|flagę INT]]

Flaga IF pozwala kontrolować czy procesor ma obsługiwać przerwania czy nie

1. odkłada na [[Stos]] flagi i następną instrukcję.
2. Pobiera z *Tablicy deskryptorów* adres *Procedury obsługi*
3. Wykonuje
4. Odzyskuje zapisany stan procesora i wraca do przerwanego podprogramu [[Najważniejsze instrukcje|rozkazem]] `iret`, następnie wysyła sygnał EOI ^[End Of Interrupt] do [[#Układ 8259]]: kontynuuj obsługę przerwań.

# Układ 8259
Zajmuje się priorytetyzacją obsługi równocześnych przerwań z różnych urządzeń.
>[!tip] Może przerwać obsługę przerwania

Priorytety są programowalne.

## APIC

Układy można *kaskadować* w ramach układu APIC. APIC-i mogą być właściwe dla każdego rdzenia procesora. 
Zajmuje się mapowaniem kodu przerwania IRQ^[Interrupt Request] na numer deskryptora^[Różne numery w różnych OS-ach!] w tablicy przerwań.

# 
---
## System symetryczny
Każdy^[[[#^b1cb5e]]] procesor może realizować obsługę przerwania.
- Windows
Programista *może* zlecić wykonanie konkretnemu procesorowi.

>[!warning] System Windows *nie dopuszcza* zagnieżdżonego wywołania przerwań o niższym priorytecie!
>Wywołane "podprzerwanie" nigdy nie zostanie dopuszczone do obsługi, co zawiesi *system operacyjny*(!)
## System asymetryczny
Jeden procesor obsługuje przerwania [[OS]], reszta przerwania użytkownika.
- Niektóre distra Linuxa (głównie w systemach klastrowych)

>[!warning] Przerwania wywołane zegarem systemowym obsługuje tylko dedykowany procesor!

^b1cb5e

# 
---
## Maskowalne
## Niemaskowalne



# Wyjątki procesora
## Niepowodzenia (Faults)
Recoverable usterki.
## Pułapki (Traps)
Stany kontrolowanej bezczynności, m.in. breakpointy debuggera.
## Błędy nienaprawialne (Aborts)

## 
![[AKO_2024_cz_4.pdf#page=72]]

# DMA
Direct Memory Access: urządzenie które wyręcza procesor w komunikacji RAM - IO. 