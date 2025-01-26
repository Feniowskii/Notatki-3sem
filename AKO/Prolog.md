
```asm
_moja_funkcja PROC:
             ; PROLOG
push ebp     ; zapamiętaj ebp wywołującego
mov ebp, esp ; zastosuj esp jako swój ebp
sub esp, ... ; zarezerwuj bajty na stosie na własny użytek
push eax     ;
push ebx     ; zapamiętaj zastane wartości rejestrów wołąjącego

...          

             ; EPILOG
pop ebx      ;
pop eax      ; przywróć zastane rejestry
add esp, ... ; oddaj zaarezerwowany stos
pop ebp      ; oddaj wołającemu jego ebp
ret          ; powróć do instrukcji z wierzchołka stosu
ENDP
```

>[!Tip] Epilog wykonuje się w odwrotnej kolejności co Prolog
>Zgodnie z ideą [[Stos|stosu]].