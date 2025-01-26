*Procesor* wyposażony jest w wiele grup rejestrów. Na Ako korzystamy z *rejestrów ogólnego przeznaczenia*. Traktujemy je jako lokalne zmienne procesora. Dzięki nim ograniczamy dostępy do [[Pamięć fizyczna|Pamięci]].
#
---

# 16-bit
Od dawna przestarzały, będziemy go używać na kursie.
#
---
# 32-bit
## Rejestry ogólne
`eax, ebx, ecx, edx`
`ah, al`
`bh, bl`
`eax`: od 0 do 31
`ax`: od 0 do 15 \[0, 15)
`ah`: (high quarter) \[8,16) (1/4 `eax`)
`al`: (low quarter) \[0,8)

>[!Warning]
>Zczytując 1 bajt do *starszej* części rejestru niższe podrejestry będą uzupełnione następnymi blokami pamięci!

## Rejestry szczególne (konwencjonalne)
- `esi`, `edi`: indeksy
- `ebp`: Rejestr bazowy (*base pointer*)

`esp`: [[Stos|Stack]] pointer
`eip`: READ ONLY ^[[[Najważniejsze instrukcje#^909b56]]]
 instruction pointer
#
---

# 64-bit
Nie ma wyższych ćwiartek[^ćwiartki] (8-16) (są, ale nie są polecane, jest na to czarna magia)

%% #todo Konieczny link do slajdu *Rejestry ogólnego przeznaczenia (64-bitowe) (5)* %%
#
---

# [[Flagi|Rejestr stanu procesora]]

[^ćwiartki]: 1/4 32 = 1/8 64