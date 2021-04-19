# CHANGELOG

Il file di **Changelog** raccoglie tutte le modifiche (presenti e future) ai file pubblicati. Il file di **Changelog** sostituisce la **Roadmap** precedentemente pubblicata.

## Prossimi aggiornamenti

## 20/04/2021
Aggiunti i campi **categoria_60_69**, **categoria_70_79** e **categoria_soggetti_fragili** all'interno dei file `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo Dati | Descrizione |
|--|--|--|
| categoria_70_79 | integer | Numero somministrazioni effettuate ai soggetti con età anagrafica compresa tra 70 e 79 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_60_69 | integer | Numero somministrazioni effettuate ai soggetti con età anagrafica compresa tra 60 e 69 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_soggetti_fragili | integer | Numero di somministrazioni effettuate ai soggetti fragili e loro caregiver indicate per giorno, regione e fascia d'età. |

La **categoria_forze_armate** indicherà il totale delle somministrazioni effettuate al personale del Comparto Difesa e Sicurezza.

**TBD**
Il file `punti-somministrazione-latest` sarà dismesso nei prossimi giorni.

## 24/03/2021
Aggiunta la categoria relativa alle altre somministrazioni (**categoria_altro**), scorporata dalla categoria del personale non sanitario. Il campo è stato aggiunto ai seguenti file: `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

## 25/02/2021
Aggiunto il file contenente i principali punti di somministrazione suddivisi per tipologia (`punti-somministrazione-tipologia`).

## 20/02/2021
I file contenenti le categorie prevalenti per le somministrazioni saranno estese con:
* la categoria relativa ai soggetti appartenenti alle Forze Armate (**categoria_forze_armate**)
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
