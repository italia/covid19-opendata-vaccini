
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


<table>
  <tr>
   <td colspan="3" ><strong>consegne-vaccini-latest</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Campo</strong>
   </td>
   <td><strong>Tipo di dati</strong>
   </td>
   <td><strong>Descrizione</strong>
   </td>
  </tr>
  <tr>
   <td>index
   </td>
   <td>integer
   </td>
   <td>Codice identificativo del record.
   </td>
  </tr>
  <tr>
   <td>area
   </td>
   <td>string
   </td>
   <td>Sigla della regione di consegna. 
   </td>
  </tr>
  <tr>
   <td>fornitore
   </td>
   <td>string
   </td>
   <td>Nome completo del fornitore del vaccino.
   </td>
  </tr>
  <tr>
   <td>data_consegna
   </td>
   <td>datetime
   </td>
   <td>Il giorno in cui è avvenuta la consegna.
   </td>
  </tr>
  <tr>
   <td>numero_dosi
   </td>
   <td>integer
   </td>
   <td>Il numero di dosi del vaccino consegnate in quel giorno per regione.
   </td>
  </tr>
  <tr>
   <td>codice_NUTS1
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 1.
   </td>
  </tr>
    <tr>
   <td>codice_NUTS2
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 2.
   </td>
  </tr>
    <tr>
   <td>codice_regione_ISTAT
   </td>
   <td>integer
   </td>
   <td>Codice ISTAT della Regione.
   </td>
  </tr>
    <tr>
   <td>nome_regione
   </td>
   <td>string
   </td>
   <td>Denominazione standard dell'area (dove necessario denominazione bilingue).
   </td>
  </tr>
</table>


<table>
  <tr>
   <td colspan="3" ><strong>vaccini-summary-latest</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Campo</strong>
   </td>
   <td><strong>Tipo di dati</strong>
   </td>
   <td><strong>Descrizione</strong>
   </td>
  </tr>
  <tr>
   <td>index
   </td>
   <td>integer
   </td>
   <td>Codice identificativo del record.
   </td>
  </tr>
  <tr>
   <td>area
   </td>
   <td>string
   </td>
   <td>Sigla della regione di consegna.
   </td>
  </tr>
  <tr>
   <td>ultimo_aggiornamento
   </td>
   <td>datetime
   </td>
   <td>Giorno dell’ultimo aggiornamento del totale.
   </td>
  </tr>
  <tr>
   <td>dosi_consegnate
   </td>
   <td>integer
   </td>
   <td>Numero totale di dosi di vaccino consegnate per regione.
   </td>
  </tr>
  <tr>
   <td>dosi_somministrate
   </td>
   <td>integer
   </td>
   <td>Numero totale di dosi di vaccino somministrate per regione.
   </td>
  </tr>
  <tr>
   <td>percentuale_somministrazione
   </td>
   <td>number
   </td>
   <td>Percentuale di dosi somministrate sulle dosi consegnate.
   </td>
  </tr>
   <tr>
   <td>codice_NUTS1
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 1.
   </td>
  </tr>
    <tr>
   <td>codice_NUTS2
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 2.
   </td>
  </tr>
    <tr>
   <td>codice_regione_ISTAT
   </td>
   <td>integer
   </td>
   <td>Codice ISTAT della Regione.
   </td>
  </tr>
    <tr>
   <td>nome_regione
   </td>
   <td>string
   </td>
   <td>Denominazione standard dell'area (dove necessario denominazione bilingue).
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="3" ><strong>somministrazioni-vaccini-latest</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Campo</strong>
   </td>
   <td><strong>Tipo di dati</strong>
   </td>
   <td><strong>Descrizione</strong>
   </td>
  </tr>
  <tr>
   <td>index
   </td>
   <td>integer
   </td>
   <td>Codice identificativo del record.
   </td>
  </tr>
  <tr>
   <td>area
   </td>
   <td>string
   </td>
   <td>Sigla della regione di consegna. 
   </td>
  </tr>
    <tr>
   <td>fornitore
   </td>
   <td>string
   </td>
   <td>nome completo del fornitore del vaccino.
   </td>
  </tr>
  <tr>
   <td>data_somministrazione
   </td>
   <td>datetime
   </td>
   <td>Data di somministrazione.
   </td>
  </tr>
  <tr>
   <td>fascia_anagrafica
   </td>
   <td>string
   </td>
   <td>Identifica la fascia anagrafiche in cui appartengono i soggetti a cui è stato somministrato il vaccino.
   </td>
  </tr>
  <tr>
   <td>sesso_maschile
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età.
   </td>
  </tr>
  <tr>
   <td>sesso_femminile
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età.
   </td>
  </tr>
  <tr>
   <td>categoria_operatori_sanitari_sociosanitari
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti appartenenti alla categoria degli operatori sanitari e sociosanitari a cui è stato somministrato il vaccino per giorno, regione e fascia d'età.
   </td>
  </tr>
  <tr>
   <td>categoria_personale_non_sanitario
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti appartenenti alla categoria del personale non sanitario a cui è stato somministrato il vaccino per giorno, regione e fascia d'età.
   </td>
  </tr>
  <tr>
   <td>categoria_ospiti_rsa
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti ospiti della struttura residenziale a cui è stato somministrato il vaccino per giorno, regione e fascia d'età.
   </td>
  </tr>
   <tr>
   <td>categoria_over80
   </td>
   <td>integer
   </td>
   <td>Numero somministrazioni categoria di rischio prevalente over 80 per giorno, regione e fascia d'età.
   </td>
  </tr>
    </tr>
   <tr>
   <td>prima_dose
   </td>
   <td>integer
   </td>
   <td>Numero prime somministrazioni.
   </td>
  </tr>
     <tr>
   <td>seconda_dose
   </td>
   <td>integer
   </td>
   <td>Numero seconde somministrazioni.
   </td>
  </tr>
   <tr>
   <td>codice_NUTS1
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 1.
   </td>
  </tr>
    <tr>
   <td>codice_NUTS2
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 2.
   </td>
  </tr>
    <tr>
   <td>codice_regione_ISTAT
   </td>
   <td>integer
   </td>
   <td>Codice ISTAT della Regione.
   </td>
  </tr>
    <tr>
   <td>nome_regione
   </td>
   <td>string
   </td>
   <td>Denominazione standard dell'area (dove necessario denominazione bilingue).
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="3" ><strong>somministrazioni-vaccini-summary-latest</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Campo</strong>
   </td>
   <td><strong>Tipo di dati</strong>
   </td>
   <td><strong>Descrizione</strong>
   </td>
  </tr>
  <tr>
   <td>index
   </td>
   <td>integer
   </td>
   <td>Codice identificativo del record.
   </td>
  </tr>
  <tr>
   <td>area
   </td>
   <td>string
   </td>
   <td>Sigla della regione in cui è avvenuta la somministrazione.
   </td>
  </tr>
  <tr>
   <td>data_somministrazione
   </td>
   <td>datetime
   </td>
   <td>Giorno in cui è avvenuta la somministrazione.
   </td>
  </tr>
  <tr>
   <td>totale
   </td>
   <td>integer
   </td>
   <td>Numero totale di dosi di vaccino somministrate per giorno e regione.
   </td>
  </tr>
  <tr>
   <td>sesso_maschile
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno e regione. 
   </td>
  </tr>
  <tr>
   <td>sesso_femminile
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno e regione. 
   </td>
  </tr>
  <tr>
   <td>categoria_operatori_sanitari_sociosanitari
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti appartenenti alla categoria degli operatori sanitari e sociosanitari a cui è stato somministrato il vaccino per giorno e regione. 
   </td>
  </tr>
  <tr>
   <td>categoria_personale_non_sanitario
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti appartenenti alla categoria del personale non sanitario a cui è stato somministrato il vaccino per giorno, regione e fascia d'età.
   </td>
  </tr>
  <tr>
   <td>categoria_ospiti_rsa
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti ospiti della struttura residenziale a cui è stato somministrato il vaccino per giorno e regione. 
   </td>
  </tr>
  <tr>
   <td>categoria_over80
   </td>
   <td>integer
   </td>
   <td>Numero somministrazioni categoria di rischio prevalente over 80 per giorno, regione e fascia d'età.
   </td>
  </tr>
    </tr>
   <tr>
   <td>prima_dose
   </td>
   <td>integer
   </td>
   <td>Numero prime somministrazioni.
   </td>
  </tr>
     <tr>
   <td>seconda_dose
   </td>
   <td>integer
   </td>
   <td>Numero seconde somministrazioni.
   </td>
  </tr>
   <tr>
   <td>codice_NUTS1
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 1.
   </td>
  </tr>
    <tr>
   <td>codice_NUTS2
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 2.
   </td>
  </tr>
    <tr>
   <td>codice_regione_ISTAT
   </td>
   <td>integer
   </td>
   <td>Codice ISTAT della Regione.
   </td>
  </tr>
    <tr>
   <td>nome_regione
   </td>
   <td>string
   </td>
   <td>Denominazione standard dell'area (dove necessario denominazione bilingue).
   </td>
  </tr>
</table>

<table>
  <tr>
   <td colspan="3" ><strong>punti-somministrazione-latest</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Campo</strong>
   </td>
   <td><strong>Tipo di dati</strong>
   </td>
   <td><strong>Descrizione</strong>
   </td>
  </tr>
  <tr>
   <td>area
   </td>
   <td>string
   </td>
   <td>Regione.
   </td>
  </tr>
  <tr>
   <td>provincia
   </td>
   <td>string
   </td>
   <td>Provincia.
   </td>
  </tr>
  <tr>
   <td>comune
   </td>
   <td>string
   </td>
   <td>Comune.
   </td>
  </tr>
  <tr>
   <td>presidio_ospedaliero
   </td>
   <td>string
   </td>
   <td>Presidio di somministrazione.
   </td>
  </tr>
   <tr>
   <td>codice_NUTS1
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 1.
   </td>
  </tr>
    <tr>
   <td>codice_NUTS2
   </td>
   <td>string
   </td>
   <td>Classificazione europea delle unità territoriali NUTS: livello NUTS 2.
   </td>
  </tr>
    <tr>
   <td>codice_regione_ISTAT
   </td>
   <td>integer
   </td>
   <td>Codice ISTAT della Regione.
   </td>
  </tr>
    <tr>
   <td>nome_regione
   </td>
   <td>string
   </td>
   <td>Denominazione standard dell'area (dove necessario denominazione bilingue).
   </td>
  </tr>
</table>

<table>
  <tr>
   <td colspan="3" ><strong>anagrafica-vaccini-summary-latest</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Campo</strong>
   </td>
   <td><strong>Tipo di dati</strong>
   </td>
   <td><strong>Descrizione</strong>
   </td>
  </tr>
  <tr>
   <td>fascia_anagrafica
   </td>
   <td>string
   </td>
   <td>Fascia anagrafica.
   </td>
  </tr>
  <tr>
   <td>totale
   </td>
   <td>integer
   </td>
   <td>Totale vaccini somministrati.
   </td>
  </tr>
  <tr>
   <td>sesso_maschile
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti di sesso maschile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età.
   </td>
  </tr>
  <tr>
   <td>sesso_femminile
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti di sesso femminile a cui è stato somministrato il vaccino per giorno, regione e fascia d’età.
   </td>
  </tr>
  <tr>
   <td>categoria_operatori_sanitari_sociosanitari
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti appartenenti alla categoria degli operatori sanitari e sociosanitari a cui è stato somministrato il vaccino per giorno, regione e fascia d'età.
   </td>
  </tr>
   <tr>
   <td>categoria_personale_non_sanitario
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti appartenenti alla categoria del personale non sanitario a cui è stato somministrato il vaccino per giorno, regione e fascia d'età.
   </td>
  </tr>
  <tr>
   <td>categoria_ospiti_rsa
   </td>
   <td>integer
   </td>
   <td>Totale dei soggetti ospiti della struttura residenziale a cui è stato somministrato il vaccino per giorno, regione e fascia d'età.
   </td>
  </tr>
  <tr>
   <td>categoria_over80
   </td>
   <td>integer
   </td>
   <td>Numero somministrazioni categoria di rischio prevalente over 80 per giorno, regione e fascia d'età.
   </td>
  </tr>
    </tr>
   <tr>
   <td>prima_dose
   </td>
   <td>integer
   </td>
   <td>Numero prime somministrazioni.
   </td>
  </tr>
     <tr>
   <td>seconda_dose
   </td>
   <td>integer
   </td>
   <td>Numero seconde somministrazioni.
   </td>
  </tr>
</table>

<table>
  <tr>
   <td colspan="3" ><strong>last-update-dataset</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Campo</strong>
   </td>
   <td><strong>Tipo di dati</strong>
   </td>
   <td><strong>Descrizione</strong>
   </td>
  </tr>
  <tr>
   <td>ultimo_aggiornamento
   </td>
   <td>datetime
   </td>
   <td>Data e ora di ultimo aggiornamento del dataset.
   </td>
  </tr>
</table>

# Maintainer

* datateam-opendata - utenza appertenente alla Struttura Commissariale per l'Emergenza Covid-19

# NOTE

A partire dal 18/01/2021 i dati sono in fase di consolidamento da parte delle regioni e potranno subire alcune variazioni.

# Licenza 

[Creative Commons - Attribuzione 4.0 Internazionale (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.it)

## Authors / Copyright 

2021 (c) Commissario straordinario per l'emergenza Covid-19 - Presidenza del Consiglio dei Ministri.
