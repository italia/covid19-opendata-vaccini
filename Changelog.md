CHANGELOG

Il file di **Changelog** raccoglie tutte le modifiche (presenti e future) ai file pubblicati. Il file di **Changelog** sostituisce la **Roadmap** precedentemente pubblicata.

## Prossimi aggiornamenti

## 17/02/2023
Aggiunto il valore **00-04** alla chiave **eta** che identifica la fascia anagrafica 6 mesi-4 anni, autorizzata alla somministrazione del ciclo vaccinale primario. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `platea`, `soggetti-guariti`.

Aggiunto il valore **05-11** alla chiave **categoria_prevalente** che identifica la platea di fascia anagrafica 5-11 autorizzata alla somministrazione della 1ª dose booster dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla conclusione del ciclo vaccinale primario. La modifica ha interessato il file `platea-dose-addizionale-booster`.

Aggiunto il valore **Sanofi** alla chiave **forn** che identifica il nuovo fornitore "Sanofi". La modifica ha interessato i files `consegne-vaccini-latest`, `somministrazioni-vaccini-latest`.

## 20/01/2023
Aggiunto il campo **db3** che identifica il numero di dosi di 3ª booster somministrate a soggetti che abbiano già completato il ciclo vaccinale comprensivo di 2ª dose booster, dopo un intervallo minimo di almeno quattro mesi (120 giorni) dall'ultima somministrazione. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| db3 | integer | Numero somministrazioni 3ª booster a soggetti che hanno completato il ciclo vaccinale comprensivo di 2ª dose booster, dopo un intervallo minimo di almeno quattro mesi (120 giorni) dall'ultima somministrazione.|

Aggiunto il file `platea-3a-booster` che definisce la popolazione oggetto di somministrazione di 3ª dose booster dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla somministrazione della 2ª dose booster, suddivisa per Regione/Provincia Autonoma e categoria prevalente.

**platea-3a-booster**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| categoria_prevalente | string | Categoria prevalente a cui appartengono i soggetti oggetto di 3ª booster. |
| totale_popolazione | integer | Numero totale della popolazione presente in platea oggetto di 3ª dose booster dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla somministrazione della 2ª dose booster, suddivisa per Regione/Provincia Autonoma e categoria prevalente.|

Aggiunto il campo **guariti_post_2booster** che identifica il numero di soggetti guariti dall'infezione Covid-19 da al massimo 6 mesi post 2ª dose booster. La modifica ha interessato il file `soggetti-guariti`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| guariti_post_2booster | integer |  Numero totale della popolazione guarita da al massimo 6 mesi post 2ª dose booster, per una data Regione/Provincia Autonoma e fascia d'età |

Aggiunto il file `copertura-vaccinale` che definisce la popolazione con età superiore a 60 anni che abbia ricevuto una somministrazione o sia guarita dall'infezione Covid-19 negli ultimi quattro mesi (120 giorni), suddivisa per Regione/Provincia Autonoma e fascia anagrafica.

**copertura-vaccinale**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| fascia_anagrafica | string | Fascia anagrafica della popolazione over 60 con copertura vaccinale. |
| guariti | string | Numero totale della popolazione over 60 guarita dall'infezione Covid-19 negli ultimi quattro mesi (120 giorni). |
| vaccinati | integer | Numero totale della popolazione over 60 oggetto di somministrazione di dose di vaccino anti-Covid19 negli ultimi quattro mesi (120 giorni). |

## 17/09/2022
Dismesso il campo **dbi**. 

La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

Aggiornato il valore **db2** con il numero di dosi booster immunocompromessi/second booster somministrate. La modifica ha interesserato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| db2 | integer | Numero somministrazioni dose booster immuno/second booster. |

## 20/07/2022
Dismesso il file `platea-booster-immunocompromessi`. 

Aggiornato il valore **dbi** con il numero di dosi booster/second booster somministrate a soggetti immonocompromessi/fragili. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| dbi | integer | Numero somministrazioni dose booster/second booster somministrate a soggetti immunocompromessi/fragili che hanno già completato il ciclo vaccinale primario con tre dosi, dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla dose aggiuntiva/1ª booster/ultima infezione.|


## 26/05/2022

Aggiunto il valore **guariti_post_1booster** che identifica il numero di soggetti guariti dall'infezione Covid-19 da al massimo 6 mesi post 1ª dose booster. La modifica ha interessato il file `soggetti-guariti`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| guariti_post_1booster | integer |  Numero totale della popolazione guarita da al massimo 6 mesi post 1ª dose booster, per una data Regione/Provincia Autonoma e fascia d'età |

## 20/05/2022

*Rinominato il campo **fornitore** in **forn**. La modifica ha interessato i files `consegne-vaccini-latest`, `somministrazioni-vaccini-latest`.

*Rinominato il campo **data_somministrazione** in **data**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

*Rinominato il campo **fascia_anagrafica** in **eta**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `anagrafica-vaccini-summary-latest`, `platea`, `soggetti-guariti`.

*Rinominato il campo **sesso_maschile** in **m**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

*Rinominato il campo **sesso_femminile** in **f**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

*Rinominato il campo **prima_dose** in **d1**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

*Rinominato il campo **seconda_dose** in **d2**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

*Rinominato il campo **pregressa_infezione** in **dpi**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

*Rinominato il campo **dose_addizionale_booster** in **db1**. La modifica ha interessato i files  `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

*Rinominato il campo **booster_immuno** in **dbi**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

*Rinominato il campo **d2_booster** in **db2**. La modifica ha interessato i files `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `anagrafica-vaccini-summary-latest`.

*Rinominato il campo **codice_NUTS1** in **N1**. La modifica ha interessato i files `consegne-vaccini-latest`, `vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `punti-somministrazione-tipologia`.

*Rinominato il campo **codice_NUTS2** in **N2**. La modifica ha interessato i files `consegne-vaccini-latest`, `vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `punti-somministrazione-tipologia`.

*Rinominato il campo **codice_regione_ISTAT** in **ISTAT**. La modifica ha interessato i files `consegne-vaccini-latest`, `vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `punti-somministrazione-tipologia`.

*Rinominato il campo **nome_area** in **reg**. La modifica ha interessato i files `consegne-vaccini-latest`, `vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`, `punti-somministrazione-tipologia`, `platea`, `platea-dose-addizionale-booster`, `platea-booster-immunocompromessi`, `soggetti-guariti`, `platea-second-booster`.

Di seguito un riepilogo dei campi oggetto di modifica con i files interessati dalla stessa.

| old_name | new_name | files |
| --- | --- | --- |
| fornitore | forn | `consegne-vaccini-latest` <br/> `somministrazioni-vaccini-latest`|
| data_somministrazione | data | `somministrazioni-vaccini-latest` <br/> `somministrazioni-vaccini-summary-latest`|
| fascia_anagrafica | eta | `somministrazioni-vaccini-latest`<br/> `anagrafica-vaccini-summary-latest`<br/> `platea`<br/> `soggetti-guariti`|
| sesso_maschile | m | `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `anagrafica-vaccini-summary-latest`|
| sesso_femminile | f | `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `anagrafica-vaccini-summary-latest`|
| prima_dose | d1 | `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `anagrafica-vaccini-summary-latest`|
| seconda_dose | d2 | `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `anagrafica-vaccini-summary-latest`|
| pregressa_infezione | dpi | `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `anagrafica-vaccini-summary-latest`|
| dose_addizionale_booster | db1 | `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `anagrafica-vaccini-summary-latest`|
| booster_immuno | dbi | `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `anagrafica-vaccini-summary-latest`|
| d2_booster | db2 | `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `anagrafica-vaccini-summary-latest`|
| codice_NUTS1 | N1 | `consegne-vaccini-latest`<br/> `vaccini-summary-latest`<br/> `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `punti-somministrazione-tipologia`|
| codice_NUTS2 | N2 | `consegne-vaccini-latest`<br/> `vaccini-summary-latest`<br/> `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `punti-somministrazione-tipologia`|
| codice_regione_ISTAT | ISTAT | `consegne-vaccini-latest`<br/> `vaccini-summary-latest`<br/> `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `punti-somministrazione-tipologia`|
| nome_area | reg | `consegne-vaccini-latest`<br/> `vaccini-summary-latest`<br/> `somministrazioni-vaccini-latest`<br/> `somministrazioni-vaccini-summary-latest`<br/> `punti-somministrazione-tipologia`<br/> `platea`<br/> `platea-dose-addizionale-booster`<br/> `platea-booster-immunocompromessi`<br/> `soggetti-guariti`<br/> `platea-second-booster`|

## 12/04/2022

Aggiunto il campo **d2_booster** che identifica il numero di dosi di second booster somministrate a soggetti che abbiano già completato il ciclo vaccinale comprensivo di dose booster, dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla dose booster stessa. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| d2_booster | integer | Numero somministrazioni second booster a soggetti che hanno già completato il ciclo vaccinale comprensivo di dose booster, dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla dose booster stessa.|

Aggiunto il file `platea-second-booster` che definisce la popolazione oggetto di somministrazione di second booster dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla somministrazione della prima dose booster, suddivisa per Regione/Provincia Autonoma e categoria prevalente.

**platea-second-booster**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| categoria_prevalente | string | Categoria prevalente a cui appartengono i soggetti oggetto di second booster. |
| totale_popolazione | integer | Numero totale della popolazione presente in platea oggetto di second booster dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla somministrazione della prima dose booster, suddivisa per Regione/Provincia Autonoma e categoria prevalente.|

## 01/03/2022

Aggiunto il valore **booster_immuni** che identifica il numero di dosi booster somministrate a soggetti di età pari o superiore a 12 anni, che abbiano già completato il ciclo vaccinale primario con tre dosi (di cui la terza addizionale), dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla dose addizionale stessa. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| booster_immuno | integer | Numero somministrazioni dose booster a soggetti che hanno già completato il ciclo vaccinale primario con tre dosi (di cui la terza addizionale), dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla dose addizionale stessa.|

Aggiunto il file `platea-booster-immunocompromessi` che definisce la popolazione immunocompromessa oggetto di somministrazione di dose booster a seguito del completamento del ciclo vaccinale primario con tre dosi (di cui la terza addizionale) dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla dose addizionale stessa, suddivisa per Regione/Provincia Autonoma.

**platea-booster-immunocompromessi**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| totale_popolazione | integer | Numero totale della popolazione immunocompromessa presente in platea oggetto di somministrazione di dose booster a seguito del completamento del ciclo vaccinale primario con tre dosi (di cui la terza addizionale) dopo un intervallo minimo di almeno quattro mesi (120 giorni) dalla dose addizionale stessa, diviso per Regione/Provincia Autonoma. |

## 24/02/2022

È stato dismesso il valore **totale_guariti**. La modifica ha interessato il file `soggetti-guariti`.

Sono stati aggiunti i valori **guariti_senza_somm** e **guariti_post_somm** che identificano il numero di soggetti guariti dall'infezione Covid-19 rispettivamente senza somministrazioni e post 2ª/unica dose. La modifica ha interessato il file `soggetti-guariti`.

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| guariti_senza_somm | integer | Numero totale della popolazione guarita da al massimo 6 mesi senza alcuna somministrazione, per una data Regione/Provincia Autonoma e fascia d'età |
| guariti_post_somm | integer |  Numero totale della popolazione guarita da al massimo 4 mesi post 2ª/unica dose, per una data Regione/Provincia Autonoma e fascia d'età |


## 26/11/2021
Sono stati dismessi i file `platea-dose-aggiuntiva` e `platea-dose-booster`. 

Sono stati dismessi i valori **dose_aggiuntiva** e **dose_booster**. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

Aggiunto il valore **dose_addizionale_booster** che identifica il numero di dosi addizionali/richiamo (booster) somministrate. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

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
Aggiunto il valore **dose_booster** che identifica il numero di dosi richiamo (booster) somministrate. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

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
Aggiunto il valore **dose_aggiuntiva** che identifica il numero di dosi aggiuntive somministrate. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

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
Aggiunto il valore **pregressa_infezione** che identifica il numero di somministrazioni effettuate a soggetti con pregressa infezione da covid-19 nel periodo 3-6 mesi e che, pertanto, concludono il ciclo vaccinale con un'unica dose. La modifica ha interessato i files `anagrafica-vaccini-summary-latest`, `somministrazioni-vaccini-latest`, `somministrazioni-vaccini-summary-latest`.

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
