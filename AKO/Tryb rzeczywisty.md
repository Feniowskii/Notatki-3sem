Procesor startuje program w trybie #16bit owym rzeczywistym i oddaje kontrolę w trybie #32bit owym chronionym.

# Segmenty
adres fizyczny = rejestr segmentowy<<4 + offset

Rejestry segmentowe trybu #16bit owego rzeczywistego:
- `CS` code segment
- `DS` data segment
- `ES` extra segment
	- kolejne dodatkowe segmenty `FS`, `GS`, ...
- `SS` stack segment 

# Adres logiczny
w trybie rzeczywistym adres fizyczny ma postać `segment : offset`

>[!tip] Adresowanie bezpośrednie
>Żeby zaadresować znaną komórkę pamięci w trybie #32bit owym przed adresem należy podać słowo `ds`, np:
> ```asm
> mov eax, ds:[400000h]
