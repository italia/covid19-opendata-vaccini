# CHANGELOG

Il file di **Changelog** raccoglie tutte le modifiche (presenti e future) ai file pubblicati. Il file di **Changelog** sostituisce la **Roadmap** precedentemente pubblicata.

## Prossimi aggiornamenti

**20/02/2021**

I file contenenti le categorie prevalenti per le somminitrsazioni saranno estese con:
* la categoria relativa ai soggetti appartenti alle Forze Armate (**categoria_forze_armate**)
* la categoria relativa al personale scolastico (**categoria_personale_scolastico**)


## 29/01/2021
* Verranno aggiunti i campi **codice_NUTS1**, **codice_NUTS2**, **codice_regione_ISTAT**, **nome_regione** contenenti informazioni standard relative alla dimensione geografica. Le modifiche riguarderanno i seguenti file: `consegne-vaccini-latest`, `punti-somministrazione-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `vaccini-summary-latest`. 
* rimozione di area = ITA sul file `somministrazioni-vaccini-summary-latest`
* modifiche al file README.md
* rimozione file ROADMAP.md

## 18/01/2021

Aggiunti i campi **fornitore**, **categoria_over80**, **prima_dose**, **seconda_dose** all'interno del file `somministrazioni-vaccini-latest`. 

| Campo | Tipo Dati | Descrizione |
|--|--|--|
| fornitore | string | nome completo del fornitore del vaccino |
| categoria_over80| integer | numero somministrazioni categoria di rischio prevalente over 80 |
| prima_dose| integer | numero prime somministrazioni |
| seconda_dose| integer | numero seconde somministrazioni |

L'indicazione del fornitore sarà disponibile a partire dal primo giorno di somministrazione (Vax day).

Aggiunti i campi **categoria_over80**, **prima_dose**, **seconda_dose** all'interno dei file `anagrafica-vaccini-summary-latest` e `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo Dati | Descrizione |
|--|--|--|
| categoria_over80| integer | numero somministrazioni categoria di rischio prevalente over 80 |
| prima_dose| integer | numero prime somministrazioni |
| seconda_dose| integer | numero seconde somministrazioni |


## 16/01/2021

Aggiunto il campo **fornitore** all'interno del file `consegne-vaccini-latest` indicante il nome del fornitore del vaccino
| Campo | Tipo Dati | Descrizione |
|--|--|--|
| fornitore | string | nome completo del fornitore del vaccino |
