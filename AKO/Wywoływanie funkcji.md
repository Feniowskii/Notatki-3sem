# Wywoływanie funkcji
![[Standardy wywołań.png]]

>[!Tip] Czyszczenie stosu jako program *wywołujący* (Standard C)
> ```asm
> push ... ; a
> push ... ; b
> call ...
> 
> add esp, (rozmiar a i b) ; przesuwamy wskaźnik stosu 

>[!Tip] Czyszczenie stosu jako program *wywoływany* (Standard StdCall)
>```asm
>_moja_funkcja@12 PROC
>...
>ret 12 ; wracając do wywołującego dodaj 12 do esp
>ENDP
>```
>Rozmiar sumaryczny parametrów będzie *dekoratorem* nazwy funkcji! np. `_moja_funkcja@12`

![[AKO/Prolog|Prolog]]

^5bb091

>[!info] Funkcja musi zachować wartość rejestrów:
>esp, ebp, edi, edi, ebx
>(Standard C)
>>[!warning] Można modyfikować ecx, edx
>>Na przykład [[Najważniejsze instrukcje#loop|loop]] dekrementuje ecx

^a7507b