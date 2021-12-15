<h1 align="center">Covid-19 Opendata Vaccini</h1>

<div align="center">
<img src="coccarda.png" width="150">
</div>
<div align="center">
  Questo repository contiene i dati in formato aperto relativi ai vaccini anti COVID-19
</div>
<br />


# Descrizione repository

Questo repository contiene i dati in formato aperto relativi alla consegna e somministrazione nelle varie regioni Italiane dei vaccini anti COVID-19. Il dataset è suddiviso in 10 tabelle che riguardano principalmente i dati sui vaccini rispetto a:


*   consegne suddivise per data di consegna e regione;
*   somministrazioni suddivise per data, regione, fascia d'età, genere e categoria di appartenenza del soggetto vaccinato;
*   platee di somministrazione;
*   punti di somministrazione.


# Descrizione dataset

Nella cartella dati si possono trovare 10 tabelle in formato json e csv:


*   **consegne-vaccini-latest**: dati sul totale delle consegne giornaliere dei vaccini suddivise per regioni.
*   **vaccini-summary-latest**: dati sul totale delle consegne e somministrazioni avvenute sino ad oggi, includendo la percentuale di dosi somministrate (sul totale delle dosi consegnate) suddivise per regioni.
*   **somministrazioni-vaccini-latest**: dati sulle somministrazioni giornaliere dei vaccini suddivisi per regioni e fasce d'età dei soggetti vaccinati.
*   **somministrazioni-vaccini-summary-latest**: dati sul totale delle somministrazioni giornaliere per regioni dei soggetti vaccinati.
*   **punti-somministrazione-latest**: punti di somministrazione per ciascuna Regione e Provincia Autonoma.
*   **anagrafica-vaccini-summary-latest**: totali delle somministrazioni per fasce d'età.
*   **last-update-dataset**: data e ora di ultimo aggiornamento del dataset.
*   **platea**: dati riferiti alla popolazione vaccinabile suddivisi per Regione/Provincia Autonoma e fascia d'età.
*   **platea-dose-addizionale-booster**: dati riferiti alla popolazione oggetto di dose addizionale/richiamo (booster) che ha ultimato il ciclo vaccinale dal almeno 5 mesi suddivisi per Regione/Provincia Autonoma e categoria prevalente.
*   **soggetti-guariti**: dati riferiti alla popolazione guarita dall'infezione Covid-19 da al massimo 6 mesi.


I campi di ogni tabella sono schematizzati nelle seguenti tavole:

**consegne-vaccini-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della regione di consegna. |
| fornitore | string | Nome completo del fornitore del vaccino. |
| data_consegna | datetime | Il giorno in cui è avvenuta la consegna. |
| numero_dosi | integer | Il numero di dosi del vaccino consegnate in quel giorno per regione. |
| codice_NUTS1 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | integer | Codice ISTAT della Regione. |
| nome_regione | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**vaccini-summary-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della regione di consegna. |
| ultimo_aggiornamento | datetime | Giorno dell’ultimo aggiornamento del totale. |
| dosi_consegnate | integer | Numero totale di dosi di vaccino consegnate per regione. |
| dosi_somministrate | integer | Numero totale di dosi di vaccino somministrate per regione. |
| percentuale_somministrazione | number | Percentuale di dosi somministrate sulle dosi consegnate. |
| codice_NUTS1 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | integer | Codice ISTAT della Regione. |
| nome_regione | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**somministrazioni-vaccini-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della regione di consegna. |
| fornitore | string | nome completo del fornitore del vaccino. |
| data_somministrazione | datetime | Data di somministrazione. |
| fascia_anagrafica | string | Identifica la fascia anagrafica alla quale appartengono i soggetti a cui è stato somministrato il vaccino. |
| sesso_maschile | integer | Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età. |
| sesso_femminile | integer | Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età. |
| prima_dose | integer | Numero prime somministrazioni. |
| seconda_dose | integer | Numero seconde somministrazioni. |
| pregressa_infezione | integer | Numero di somministrazioni effettuate a soggetti con pregressa infezione da covid-19 nel periodo 3-6 mesi e che, pertanto, concludono il ciclo vaccinale con un'unica dose |
| dose_addizionale_booster | integer | Numero somministrazioni dose addizionale/richiamo (booster). |
| codice_NUTS1 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | integer | Codice ISTAT della Regione. |
| nome_regione | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**somministrazioni-vaccini-summary-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della regione in cui è avvenuta la somministrazione. |
| data_somministrazione | datetime | Giorno in cui è avvenuta la somministrazione. |
| totale | integer | Numero totale di dosi di vaccino somministrate per giorno e regione. |
| sesso_maschile | integer | Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno e regione. |
| sesso_femminile | integer | Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno e regione. |
| prima_dose | integer | Numero prime somministrazioni. |
| seconda_dose | integer | Numero seconde somministrazioni. |
| pregressa_infezione | integer | Numero di somministrazioni effettuate a soggetti con pregressa infezione da covid-19 nel periodo 3-6 mesi e che, pertanto, concludono il ciclo vaccinale con un'unica dose |
| dose_addizionale_booster | integer | Numero somministrazioni dose addizionale/richiamo (booster). |
| codice_NUTS1 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | integer | Codice ISTAT della Regione. |
| nome_regione | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**punti-somministrazione-tipologia**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| area | string | Regione. |
| denominazione_struttura | string | Presidio di somministrazione. |
| tipologia | string | Tipologia del presidio di somministrazione: ospedaliero o territoriale. |
| codice_NUTS1 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 1. |
| codice_NUTS2 | string | Classificazione europea delle unità territoriali NUTS: livello NUTS 2. |
| codice_regione_ISTAT | integer | Codice ISTAT della Regione. |
| nome_regione | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |

**anagrafica-vaccini-summary-latest**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| fascia_anagrafica | string | Fascia anagrafica. |
| totale | integer | Totale vaccini somministrati. |
| sesso_maschile | integer | Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età. |
| sesso_femminile | integer | Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età. |
| prima_dose | integer | Numero prime somministrazioni. |
| seconda_dose | integer | Numero seconde somministrazioni. |
| pregressa_infezione | integer | Numero di somministrazioni effettuate a soggetti con pregressa infezione da covid-19 nel periodo 3-6 mesi e che, pertanto, concludono il ciclo vaccinale con un'unica dose |
| dose_addizionale_booster | integer | Numero somministrazioni dose addizionale/richiamo (booster). |

**last-update-dataset**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| ultimo_aggiornamento | datetime | Data e ora di ultimo aggiornamento del dataset. |

**platea**

| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| fascia_anagrafica | string | Fascia anagrafica a cui appartengono i soggetti vaccinabili. |
| totale_popolazione | integer | Numero totale della popolazione presente in platea per una data fascia d'età |

**platea-dose-addizionale-booster**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| categoria_prevalente | string | Categoria prevalente a cui appartengono i soggetti oggetto di dose addizionale/richiamo (booster). |
| totale_popolazione | integer | Numero totale della popolazione presente in platea oggetto di dose addizionale/richiamo (booster) che ha completato il ciclo vaccinale da almeno 5 mesi diviso per Regione/Provincia Autonoma, categoria prevalente. |

**soggetti-guariti**
| Campo | Tipo di dati | Descrizione |
| --- | --- | --- |
| index | integer | Codice identificativo del record. |
| area | string | Sigla della Regione/Provincia Autonoma. |
| nome_area | string | Denominazione standard dell'area (dove necessario denominazione bilingue). |
| fascia_anagrafica | string | Fascia anagrafica a cui appartengono i soggetti guariti. |
| totale_guariti | integer | Numero totale della popolazione guarita da al massimo 6 mesi, per una data fascia d'età |

# Maintainer

* datateam-opendata - utenza appertenente alla Struttura Commissariale per l'Emergenza Covid-19

# NOTE

A partire dal 18/01/2021 i dati sono in fase di consolidamento da parte delle regioni e potranno subire alcune variazioni.

# Licenza

[Creative Commons - Attribuzione 4.0 Internazionale (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.it)

## Authors / Copyright

2021 (c) Commissario straordinario per l'emergenza Covid-19 - Presidenza del Consiglio dei Ministri.
