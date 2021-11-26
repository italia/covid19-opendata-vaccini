CHANGELOG

Il file di **Changelog** raccoglie tutte le modifiche (presenti e future) ai file pubblicati. Il file di **Changelog** sostituisce la **Roadmap** precedentemente pubblicata.

## Prossimi aggiornamenti

## 26/11/2021
Sono stati dismessi i file `platea-dose-aggiuntiva` e `platea-dose-booster`. 

Sono stati dismessi i valori **dose_aggiuntiva** e **dose_booster**. La modifica interesserà i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

Aggiunto il valore **dose_addizionale_booster** che identifica il numero di dosi addizionali/richiamo (booster) somministrate. La modifica interesserà i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| dose_addizionale_booster | integer | Numero somministrazioni dose addizionale/richiamo (booster) |

Aggiunto il file `platea-dose-addizionale-booster` che definisce la popolazione oggetto di somministrazione di dose addizionale e richiamo (booster) che ha ultimato il ciclo vaccinale da almeno 5 mesi suddivisa per Regione/Provincia Autonoma e categoria prevalente.

**platea-dose-addizionale-booster**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| categoria_prevalente | string | Categoria prevalente a cui appartengono i soggetti oggetto di dose addizionale/richiamo (booster). |
| totale_popolazione | integer | Numero totale della popolazione presente in platea oggetto di dose addizionale/richiamo (booster) che ha completato il ciclo vaccinale da almeno 5 mesi diviso per Regione/Provincia Autonoma, categoria prevalente. |

## 26/11/2021
Aggiunto il file `soggetti-guariti` che definisce la popolazione guarita dall'infezione Covid-19 da al massimo 6 mesi.

**soggetti-guariti**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| fascia_anagrafica | string | Fascia anagrafica a cui appartengono i soggetti guariti. |
| totale_guariti | integer | Numero totale della popolazione guarita da al massimo 6 mesi, per una data fascia d'età |

## 21/10/2021
Aggiunto il valore **dose_booster** che identifica il numero di dosi richiamo (booster) somministrate. La modifica interesserà i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| dose_booster | integer | Numero somministrazioni dose richiamo (booster) |

Aggiunto il file `platea-dose-booster` che definisce la popolazione oggetto di somministrazione di dose richiamo (booster) che ha ultimato il ciclo vaccinale da almeno 6 mesi suddivisa per Regione/Provincia Autonoma e categoria prevalente.

**platea-dose-booster**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| categoria_prevalente | string | Categoria prevalente a cui appartengono i soggetti oggetto di dose richiamo (booster). |
| totale_popolazione | integer | Numero totale della popolazione presente in platea oggetto di dose richiamo (booster) che ha completato il ciclo vaccinale da almeno 6 mesi diviso per Regione/Provincia Autonoma, categoria prevalente. |

## 20/09/2021
Aggiunto il valore **dose_aggiuntiva** che identifica il numero di dosi aggiuntive somministrate. La modifica interesserà i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| dose_aggiuntiva | integer | Numero somministrazioni dose aggiuntiva |

Aggiunto il file `platea-dose-aggiuntiva` che definisce la popolazione oggetto di somministrazione di dose aggiuntiva suddivisa per Regione/Provincia Autonoma e categoria prevalente.

**platea-dose-aggiuntiva**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| categoria_prevalente | string | Categoria prevalente a cui appartengono i soggetti oggetto di dose aggiuntiva. |
| totale_popolazione | integer | Numero totale della popolazione presente in platea oggetto di dose aggiuntiva per Regione/Provincia Autonoma, categoria prevalente. |

## 05/07/2021
Aggiunto il valore **pregressa_infezione** che identifica il numero di somministrazioni effettuate a soggetti con pregressa infezione da covid-19 nel periodo 3-6 mesi e che, pertanto, concludono il ciclo vaccinale con un'unica dose. La modifica interesserà i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| pregressa_infezione | integer | Numero di somministrazioni effettuate a soggetti con pregressa infezione da covid-19 nel periodo 3-6 mesi e che, pertanto, concludono il ciclo vaccinale con un'unica dose |

## 02/06/2021
Il valore **16-19** per il campo 'fascia_anagrafica' è stato modificato in **12-19**. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`.

Aggiunto il file `platea` che definisce la popolazione interessata a ciclo vaccinale suddivisa per Regione/Provincia Autonoma e fascia d'età.

**platea**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| fascia_anagrafica | string | Fascia anagrafica a cui appartengono i soggetti vaccinabili. |
| totale_popolazione | integer | Numero totale della popolazione presente in platea per una data fascia d'età |

## 28/05/2021
La pubblicazione dei dati è stata ricondotta alla sola fascia d'età. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

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
