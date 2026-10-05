# VUT FEKT záznamy z kovidu (BPC-ALD & BPC-LOS)
Web pro lepší sledování záznamů přednášek a cvičení z předmětů BPC-ALD a BPC-LOS (VUT FEKT), které byly nahrány za kovidu.

🌐 **Web:** https://jakuslam.github.io/VUT_FEKT_ALD_zaznamy_kovid/

## Podrobněji
Tento projekt je jednoduchá statická html stránka, která má sloužit pro lepší přístup k přednáškám a cvičením Ing. Petra Petyovského, Ph.D., které byly nahrány za kovidu. Není to oficiální zdroj, pouze studentský projekt.

### Předměty
- **BPC-ALD** (Algoritmy a datové struktury): přednášky a cvičení 2021, přednášky 2022
- **BPC-LOS** (Logické obvody a systémy): přednášky a cvičení 2020 a 2021

### Funkce
- filtrování podle semestru a typu (přednášky / cvičení)
- vlastní přehrávač videa s náhledem při posunu, změnou rychlosti a celou obrazovkou
- klávesové zkratky: `mezerník` přehrát/pauza, `←`/`A` a `→`/`D` posun o 5 s, `F` celá obrazovka, `Esc` zavřít
- světlý a tmavý režim

## Struktura
| Soubor | Popis |
|---|---|
| `index.html` | rozcestník mezi předměty |
| `ald.html` | záznamy BPC-ALD |
| `los.html` | záznamy BPC-LOS |

Videa jsou uložená v poli `videa` na začátku `<script>` v souboru daného předmětu. Nové video se přidá jedním řádkem ve tvaru:
```js
{ predmet:'bpc-ald', semestr:2022, ep:1, typ:'prednaska', nazev:'Přednáška #1', delka:'1:41:00', url:'https://…', temata:'…' },
```

PS: Pokud máte nějaký nápad na zlepšení, neváhejte se mi ozvat.
