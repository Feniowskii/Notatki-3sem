# Program counter
> wskaźnik instrukcji/licznik rozkazów

Określa położenie *kolejnej* [[Instrukcja|instrukcji]].
[[Rejestry]] `eip` (32-bit) `rip` (64-bit) trzymają [[Pamięć fizyczna|adres]] komórki z następną instrukcją.
Po zczytaniu procesor już prosi [[Pamięć fizyczna]] o kolejny rozkaz.

%%
#todo Dodać slajd: Uproszczony cykl rozkazowy (5)
%%

*Rozkaz sterujący* (skokowy) zmieni `eip` po wykonaniu.
> np. branch, jump, itp.

Rozkaz sterujący *warunkowy* wykona skok jeśli spełniony jest pewien warunek. Najczęściej warunek musi zostać obliczony wcześniej innymi instrukcjami. 

*Niesterujący* zwiększy licznik po odkodowaniu.
*Zwiększy*, nie zinkrementuje! Zwiększy się o długość instrukcji i argumentów.