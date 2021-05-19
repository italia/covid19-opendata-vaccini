
<h1 align="center">Covid-19 Opendata Vaccini</h1>

<div align="center">
<img src="logo.png" width="150">
</div>
<div align="center">
  Questo repository contiene i dati in formato aperto relativi ai vaccini anti COVID-19
</div>
<br />


# Descrizione repository

Questo repository contiene i dati in formato aperto relativi alla consegna e somministrazione nelle varie regioni Italiane dei vaccini anti COVID-19. Il dataset è suddiviso in 6 tabelle che riguardano principalmente i dati sui vaccini rispetto a:


*   consegne suddivise per data di consegna e regione;
*   somministrazioni suddivise per data, regione, fascia d'età, genere e categoria di appartenenza del soggetto vaccinato;
*   punti di somministrazione.


# Descrizione dataset

Nella cartella dati si possono trovare 6 tabelle in formato json e csv:


*   **consegne-vaccini-latest**: dati sul totale delle consegne giornaliere dei vaccini suddivise per regioni.
*   **vaccini-summary-latest**: dati sul totale delle consegne e somministrazioni avvenute sino ad oggi, includendo la percentuale di dosi somministrate (sul totale delle dosi consegnate) suddivise per regioni.
*   **somministrazioni-vaccini-latest**: dati sulle somministrazioni giornaliere dei vaccini suddivisi per regioni, fasce d'età e categorie di appartenenza dei soggetti vaccinati.
*   **somministrazioni-vaccini-summary-latest**: dati sul totale delle somministrazioni giornaliere per regioni e categorie di appartenenza dei soggetti vaccinati.
*   **punti-somministrazione-latest**: punti di somministrazione per ciascuna Regione e Provincia Autonoma.
*   **anagrafica-vaccini-summary-latest**: totali delle somministrazioni per fasce d'età.
*   **last-update-dataset**: data e ora di ultimo aggiornamento del dataset.

I campi di ogni tabella sono schematizzati nelle seguenti tavole:

**consegne-vaccini-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | Integer | Codice identificativo del record. |
| area | String | Sigla della regione di consegna. |
| fornitore | String | Nome completo del fornitore del vaccino. |
| data_consegna | Datetime | Il giorno in cui è avvenuta la consegna. |
| numero_dosi | Integer | Il numero di dosi del vaccino consegnate in quel giorno per regione. |
| codice_NUTS1 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | Integer | Codice ISTAT della Regione. |
| nome_regione | String | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**vaccini-summary-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | Integer | Codice identificativo del record. |
| area | String | Sigla della regione di consegna. |
| ultimo_aggiornamento | Datetime | Giorno dell’ultimo aggiornamento del totale. |
| dosi_consegnate | Integer | Numero totale di dosi di vaccino consegnate per regione. |
| dosi_somministrate | Integer | Numero totale di dosi di vaccino somministrate per regione. |
| percentuale_somministrazione | number | Percentuale di dosi somministrate sulle dosi consegnate. |
| codice_NUTS1 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | Integer | Codice ISTAT della Regione. |
| nome_regione | String | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**somministrazioni-vaccini-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | Integer | Codice identificativo del record. |
| area | String | Sigla della regione di consegna. |
| fornitore | String | nome completo del fornitore del vaccino. |
| data_somministrazione | Datetime | Data di somministrazione. |
| fascia_anagrafica | String | Identifica la fascia anagrafiche in cui appartengono i soggetti a cui è stato somministrato il vaccino. |
| sesso_maschile | Integer | Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età. |
| sesso_femminile | Integer | Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età. |
| categoria_over80 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica maggiore o uguale a 80 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_soggetti_fragili | Integer | Numero di somministrazioni effettuate ai soggetti fragili e loro caregiver indicate per giorno, regione e fascia d'età. |
| categoria_operatori_sanitari_sociosanitari | Integer | Numero di somministrazioni effettuate agli operatori sanitari e sociosanitari indicate per giorno, regione e fascia d'età. |
| categoria_personale_non_sanitario | Integer | Numero di somministrazioni effettuate al personale non sanitario impiegato in strutture sanitarie e in attività lavorativa a rischio indicate per giorno, regione e fascia d'età. |
| categoria_ospiti_rsa | Integer | Numero di somministrazioni effettuate ai soggetti ospiti di comunità residenziali indicate per giorno, regione e fascia d'età. |
| categoria_70_79 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica compresa tra 70 e 79 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_60_69 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica compresa tra 60 e 69 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_personale_scolastico | Integer | Numero di somministrazioni effettuate al personale scolastico indicate per giorno, regione e fascia d'età. |
| categoria_forze_armate | Integer | Numero di somministrazioni effettuate al personale del comparto difesa e sicurezza indicate per giorno, regione e fascia d'età. |
| categoria_altro | Integer | Numero di somministrazioni effettuate ai soggetti non riconducibili alle precedenti categorie indicate per giorno, regione e fascia d'età. |
| prima_dose | Integer | Numero prime somministrazioni. |
| seconda_dose | Integer | Numero seconde somministrazioni. |
| codice_NUTS1 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | Integer | Codice ISTAT della Regione. |
| nome_regione | String | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**somministrazioni-vaccini-summary-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | Integer | Codice identificativo del record. |
| area | String | Sigla della regione in cui è avvenuta la somministrazione. |
| data_somministrazione | Datetime | Giorno in cui è avvenuta la somministrazione. |
| totale | Integer | Numero totale di dosi di vaccino somministrate per giorno e regione. |
| sesso_maschile | Integer | Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno e regione. |
| sesso_femminile | Integer | Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno e regione. |
| categoria_over80 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica maggiore o uguale a 80 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_soggetti_fragili | Integer | Numero di somministrazioni effettuate ai soggetti fragili e loro caregiver indicate per giorno, regione e fascia d'età. |
| categoria_operatori_sanitari_sociosanitari | Integer | Numero di somministrazioni effettuate agli operatori sanitari e sociosanitari indicate per giorno, regione e fascia d'età. |
| categoria_personale_non_sanitario | Integer | Numero di somministrazioni effettuate al personale non sanitario impiegato in strutture sanitarie e in attività lavorativa a rischio indicate per giorno, regione e fascia d'età. |
| categoria_ospiti_rsa | Integer | Numero di somministrazioni effettuate ai soggetti ospiti di comunità residenziali indicate per giorno, regione e fascia d'età. |
| categoria_70_79 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica compresa tra 70 e 79 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_60_69 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica compresa tra 60 e 69 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_personale_scolastico | Integer | Numero di somministrazioni effettuate al personale scolastico indicate per giorno, regione e fascia d'età. |
| categoria_forze_armate | Integer | Numero di somministrazioni effettuate al personale del comparto difesa e sicurezza indicate per giorno, regione e fascia d'età. |
| categoria_altro | Integer | Numero di somministrazioni effettuate ai soggetti non riconducibili alle precedenti categorie indicate per giorno, regione e fascia d'età. |
| prima_dose | Integer | Numero prime somministrazioni. |
| seconda_dose | Integer | Numero seconde somministrazioni. |
| codice_NUTS1 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | Integer | Codice ISTAT della Regione. |
| nome_regione | String | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**punti-somministrazione-tipologia**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| area | String | Regione. |
| denominazione_struttura | String | Presidio di somministrazione. |
| tipologia | String | Tipologia del presidio di somministrazione: ospedaliero o territoriale. |
| codice_NUTS1 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | String | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | Integer | Codice ISTAT della Regione. |
| nome_regione | String | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**anagrafica-vaccini-summary-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| fascia_anagrafica | String | Fascia anagrafica. |
| totale | Integer | Totale vaccini somministrati. |
| sesso_maschile | Integer | Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età. |
| sesso_femminile | Integer | Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età. |
| categoria_over80 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica maggiore o uguale a 80 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_soggetti_fragili | Integer | Numero di somministrazioni effettuate ai soggetti fragili e loro caregiver indicate per giorno, regione e fascia d'età. |
| categoria_operatori_sanitari_sociosanitari | Integer | Numero di somministrazioni effettuate agli operatori sanitari e sociosanitari indicate per giorno, regione e fascia d'età. |
| categoria_personale_non_sanitario | Integer | Numero di somministrazioni effettuate al personale non sanitario impiegato in strutture sanitarie e in attività lavorativa a rischio indicate per giorno, regione e fascia d'età. |
| categoria_ospiti_rsa | Integer | Numero di somministrazioni effettuate ai soggetti ospiti di comunità residenziali indicate per giorno, regione e fascia d'età. |
| categoria_70_79 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica compresa tra 70 e 79 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_60_69 | Integer | Numero somministrazioni effettuate ai soggetti con età anagrafica compresa tra 60 e 69 anni, non appartenenti ad altre categorie prioritarie ma ricevono la somministrazione esclusivamente sul criterio dell'età anagrafica, indicate per giorno, regione. |
| categoria_personale_scolastico | Integer | Numero di somministrazioni effettuate al personale scolastico indicate per giorno, regione e fascia d'età. |
| categoria_forze_armate | Integer | Numero di somministrazioni effettuate al personale del comparto difesa e sicurezza indicate per giorno, regione e fascia d'età. |
| categoria_altro | Integer | Numero di somministrazioni effettuate ai soggetti non riconducibili alle precedenti categorie indicate per giorno, regione e fascia d'età. |
| prima_dose | Integer | Numero prime somministrazioni. |
| seconda_dose | Integer | Numero seconde somministrazioni. |

**last-update-dataset**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| ultimo_aggiornamento | Datetime | Data e ora di ultimo aggiornamento del dataset. |


# Maintainer

* team Struttura Commissariale per l'Emergenza Covid-19


# Licenza

[Creative Commons - Attribuzione 4.0 Internazionale (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.it)

## Authors / Copyright

2021 (c) Commissario straordinario per l'emergenza Covid-19 - Presidenza del Consiglio dei Ministri.
