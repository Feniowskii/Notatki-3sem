# ERD
```mermaid
erDiagram

ZAKLAD {
	string nazwa
	string adres
}

CELA {
	int numer
	int lozka
}

BLOK {
	string nazwa
	bool zaostrzony_rygor
}

"DANE PERSONALNE" {
	string imie
	string nazwisko
	int pesel
}

OSADZONY {
	date start_wyroku
	float lata_odsiedziane
	bool niebezpieczny
}

"GRUPA PRZESTĘPCZA" {
	string nazwa
}

STRAZNIK {
	string stopien
}

%% ======= Relacje ======= %%

ZAKLAD }|--|| "BLOK": "jest częścią"

STRAZNIK ||--|| "DANE PERSONALNE": "posiada"

CELA ||--o{ OSADZONY: "zajmuje"
CELA }|--|| BLOK: "jest częścią"
STRAZNIK }o--|| BLOK: "obecnie pracuje w"
STRAZNIK }o--|{ BLOK: "ma uprawnienia do pracy w"

OSADZONY }o--o{ "GRUPA PRZESTĘPCZA": "jest członkiem"
OSADZONY ||--|| "DANE PERSONALNE": "posiada"
OSADZONY |o--o{ "GRUPA PRZESTĘPCZA": "jest liderem"
```
# Dokument
[Overleaf](https://www.overleaf.com/project/6700f2814915a287f52c9e74)
[dbdiagram.io](https://dbdiagram.io/d/Wiezienie-6713536097a66db9a3875c57) ^56826c

Jeżeli zabraknie encji:
dodać pole "zwolnienie warunkowe" do więźnia, dodać transakcję biznesową "wniosek o zwolnienie" czy coś między więźniem a pracownikiem administracyjnym. Uwaga: utrudni to zapis początku i końca wyroku.