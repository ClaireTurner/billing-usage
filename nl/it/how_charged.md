---

copyright:
  years: 2015, 2019
lastupdated: "2019-06-03"

keywords: pricing, billing, payment, charges, pricing plan, service cost, cost

subcollection: billing-usage

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:new_window: target="_blank"}


# Modalità degli addebiti a tuo carico
{: #charges}

Gli addebiti variano a seconda delle risorse utilizzate da una specifica opzione di servizio, runtime, contenitore o supporto. Le risorse possono essere il numero di chiamate API, il numero di istanze, la memoria o l'archiviazione. {{site.data.keyword.Bluemix}} fornisce degli stimatori del costo dettagliati per aiutarti a pianificare i tuoi addebiti.
{:shortdesc}


Dopo aver creato le tue risorse , puoi controllare il costo effettivo. Vai a **Gestisci > Fatturazione e utilizzo** e seleziona **Utilizzo**. Con un account fatturabile {{site.data.keyword.Bluemix_notm}}, gli addebiti a tuo carico sono basati sul calcolo, sui contenitori e sui servizi utilizzati dalla tua organizzazione. Potresti essere invitato da altri utenti {{site.data.keyword.Bluemix_notm}}
a partecipare ad organizzazioni sotto un account differente. L'utilizzo delle applicazioni o dei servizi che utilizzi nelle organizzazioni a cui sei invitato vengono addebitati all'account che contiene tali organizzazioni. Puoi visualizzare ulteriori informazioni su uno specifico addebito dalla pagina dei dettagli di ciascuna risorsa

Vengono applicati diversi tipi di addebiti a seconda delle funzioni di {{site.data.keyword.Bluemix_notm}} che stai utilizzando. La seguente tabella fornisce una panoramica di alto livello:

| Tipo di addebito | Descrizione      | Tipo di risorsa            | Esempio                  |
|----------------|------------------|--------------------------|--------------------------|
| Fisso          | Il prezzo forfettario è basato su un addebito mensile concordato che non viene adeguato. | Servizi  | Per i server Bare Metal, sono disponibili dei piani fissi da cui scegliere e tali piani vengono addebitati a una tariffa mensile fissa. |
| Misurato        | Il prezzo a utilizzo misurato è basato sul numero di GB-ore utilizzati per i runtime e sul numero di indirizzi IP e archiviazione per i contenitori. | Servizi, elaborazione e contenitori | Per il servizio Push, la quota di utilizzo che supera la franchigia mensile viene addebitata. |
| A livelli         | Alcuni piani prezzi sono basati su un modello di prezzi a livelli, quindi puoi ottenere uno sconto basato sui
volumi in base al tuo utilizzo effettivo. I servizi possono offrire dei piani prezzi di livello a blocchi, graduale o semplice. | Servizi | Il prezzo a livelli viene di norma utilizzato per le metriche di addebito di cui è prevista una quantità elevata al mese, come le chiamate API. |
| Riservato       | Il prezzo riservato è basato su un impegno a lungo termine per un servizio, in modo da consentirti di ottenere un prezzo scontato. Con un piano riservato, ottieni un'istanza del servizio dedicato facile da configurare, distribuire e consegnare in ambiente {{site.data.keyword.Bluemix_notm}} pubblico. | Servizi | DB2 on Cloud ha dei piani riservati.|
{:caption="Tabella 1. Addebiti basati sulle funzioni" caption-side="top"}


## Piani Lite
{: #liteplans}

I piani Lite sono strutturati come una quota gratuita. Puoi lavorare tranquillamente sui tuoi progetti senza il rischio di generare una fattura accidentale. La quota potrebbe essere applicabile per un periodo di tempo specifico, ad esempio un mese, o su una base di utilizzo una tantum. Il seguente elenco fornisce alcuni esempi di quote del piano Lite:

   * Numero massimo di dispositivi registrati
   * Numero massimo di bind di applicazione
   * Limite di archiviazione di dati crittografati, ad esempio 1 GB
   * Capacità produttiva fornita

Puoi facilmente trovare i servizi per i piani Lite nel catalogo. Per impostazione predefinita, tutti i servizi con un piano Lite vengono visualizzati con una tag Lite ![Tag Lite](../icons/Lite.svg). Seleziona un servizio per visualizzare i dettagli della quota per il piano Lite associato.


## Addebiti per le risorse di elaborazione
{: #compute}

L'addebito a tuo carico è basato sul tempo di esecuzione delle tue applicazioni e sulla memoria utilizzata, in *GB-ore*. GB-ore è il calcolo del numero di istanze dell'applicazione, moltiplicato per la memoria per ogni singola istanza, moltiplicato per le ore di esecuzione delle istanze. Puoi personalizzare il numero di
istanze e la quantità di memoria per ogni singola istanza in base alle tue
esigenze. Puoi anche aggiungere memoria o istanze per eseguire un ridimensionamento per un numero maggiore di utenti. Per ottenere l'importo addebitato, prendi le tue istanze dell'applicazione moltiplicate per la memoria per ogni singola istanza e per le ore di esecuzione.

Considera, ad esempio, un runtime che costa $0,07 per ogni GB-ora in due istanze da 512 MB, in esecuzione per 30 giorni (720 ore). Queste risorse costerebbero $24,15 USD, compresa la franchigia di 375 GB-ore, con i seguenti calcoli:

```
2 istanze x 0,5 GB x 720 ore = 720 GB-ore.
(720 - 375) GB-ore x $0,07 per GB-ora = $24,15
```

## Addebiti per i servizi
{: #charges-services}

Molti servizi
includono delle franchigie mensili. L'utilizzo dei servizi non inclusi come parte della franchigia viene addebitato in uno dei seguenti modi:
<dl>
<dt>Addebiti fissi</dt>
    <dd>Selezioni un piano e paghi in base a una tariffa forfettaria. Ad esempio, i server Bare Metal vengono addebitati a una tariffa forfettaria.</dd>
<dt>Addebiti misurati</dt>
    <dd>Paghi in base al consumo che fai di runtime e servizi. Ad esempio, con il
servizio Push, la quota di utilizzo che supera la franchigia mensile viene
addebitata.</dd>
<dt>Addebiti riservati</dt>
    <dd><p>In quanto proprietario di un account Pagamento a consumo o di un account Sottoscrizione, puoi riservare un'istanza del servizio, con un impegno a lungo termine, per un prezzo scontato. Ad esempio, puoi riservare l'offerta standard DB2 on Cloud di grandi dimensioni per 12 mesi.</p>
    <p>Alcuni servizi {{site.data.keyword.Bluemix_notm}} offrono dei piani riservati. Puoi richiedere un piano riservato dal catalogo {{site.data.keyword.Bluemix_notm}} facendo clic sul tile del servizio. Seleziona quindi il piano di servizio che meglio soddisfa le tue esigenze. Se è disponibile un piano riservato, fai clic su <strong>Richiesta</strong> e attieniti alle richieste che ti vengono presentate per inviare la tua richiesta. Ricevi un'e-mail che contiene le informazioni sul prezzo del piano riservato. Vieni inoltre contattato al più presto da un rappresentante del settore Vendite di {{site.data.keyword.Bluemix_notm}} per completare l'acquisto.</p></dd>
<dt>Addebiti a livelli</dt>
    <dd>Analogamente agli addebiti misurati, paghi in base al tuo consumo di runtime e servizi. Tuttavia, gli addebiti a livelli aggiungono degli ulteriori livelli di prezzo, spesso offrendo degli addebiti scontati nei livelli con un più ampio consumo. Il prezzo a livelli è offerto in modalità semplice, graduale o a blocchi.</dd>
</dl>

### Livello semplice
{: #simple_tier}

Nel modello di livello semplice, il prezzo unitario è determinato
dal livello in cui rientra la quantità da te utilizzata. Il prezzo totale è tale quantità moltiplicata per il prezzo unitario nel livello di competenza, ad esempio:

| Quantità di elementi   | Prezzo unitario per tutti gli elementi |
|---------------------|--------------------------|
| Livello 1: 1 - 1000    | $1 USD                   |
| Livello 2: 1001 - 2000 | $0,90 USD                |
| Livello 3: 2001 - 3000 | $0,75 USD                |
| Livello 4: 3001 - 4000 | $0,60 USD                |
| Livello 5: &gt; 4000   | $0,40 USD                |
{:caption="Tabella 2. Tabella prezzi di livello semplice" caption-side="top"}

La seguente tabella
illustra quanto paghi con un piano basato su un modello di prezzi di livello semplice:

| Quantità di elementi   | Calcolo dell'addebito | Prezzo totale |
|-------------------|--------------------|-------------|
| 500               | 500 × 1 = 500      | $500 USD    |
| 1500              | 1500 × 0,90 = 1350 | $1350 USD   |
| 2500              | 2500 × 0,75 = 1875 | $1875 USD   |
| ...               | ...                | ...         |
| 5200              | 5200 × 0,40 = 2080 | $2080 USD   |
{:caption="Tabella 3. Calcolo dell'addebito utilizzando un modello di prezzi di livello semplice" caption-side="top"}

### Livello graduale
{: #graduated_tier}

Nel modello di livello graduale, il prezzo unitario per livello si riduce
man mano che il tuo livello di utilizzo aumenta. Il prezzo totale è dato dagli addebiti cumulativi per ciascun livello di utilizzo, che consiste nella tua quantità moltiplicata per il prezzo unitario al livello di competenza, ad esempio:

| Quantità di elementi   |	Prezzo unitario per gli elementi nel livello|
|---------------------|---------------------------------|
| Livello 1: 1 - 1000    |	$1 USD                          |
| Livello 2: 1001 - 2000 |	$0,90 USD                       |
| Livello 3: 2001 - 3000 |	$0,75 USD                       |
| Livello 4: 3001 - 4000 |	$0,60 USD                       |
| Livello 5: &gt; 4000   |	$0,40 USD                       |
{:caption="Tabella 4. Tabella prezzi di livello graduale" caption-side="top"}

La seguente tabella
illustra quanto paghi con un piano basato su un modello di prezzi di livello graduale:

| Quantità di elementi   | Calcolo dell'addebito                                                               | Prezzo totale |
|------------------|----------------------------------------------------------------------------------|-------------|
| 500              | 500 × 1 (prezzo unitario per il livello 1) = 500                                            |	$500 USD    |
| 1500             | (1000 × 1 (prezzo unitario per il livello 1)) + (500 × 0,90 (prezzo unitario per il livello 2)) = 1450 |	$1450 USD   |
| 2500             | (1000 × 1 (prezzo unitario per il livello 1)) + (1000 × 0,90 (prezzo unitario per il livello 2)) + (500 × 0,75 (prezzo unitario per il livello 3)) = 2275 | $2275 USD |
| ...              | ...                                                                              | ...         |
| 5200             | (1000 × 1 (prezzo unitario per il livello 1)) + (1000 × 0,90 (prezzo unitario per il livello 2)) + (1000 × 0,75 (prezzo unitario per il livello 3)) + (1000 × 0,60 (prezzo unitario per il livello 4)) + (1200 × 0,40 (prezzo unitario per il livello 5)) = 3730 | $3730 USD |
{:caption="Tabella 5. Calcolo dell'addebito utilizzando un modello di prezzi di livello graduale" caption-side="top"}

### Livello a blocchi
{: #block_tier}

Nel modello di livello a blocchi, il prezzo è un addebito fisso per la
quantità da te impiegata entro uno specifico livello di utilizzo. Il prezzo totale è l'addebito per il tuo livello di utilizzo, indipendentemente dal tuo utilizzo effettivo. Ogni livello
successivo fornisce un rapporto prezzo-quantità più basso. Ad esempio:

| Quantità di elementi   |	Prezzo totale per tutti gli elementi |
|---------------------|---------------------------|
| Livello 1: &lt;= 1000  |	$1000 USD                 |
| Livello 2: &lt;= 2000  |	$1900 USD                 |
| Livello 3: &lt;= 3000  |	$2800 USD                 |
| Livello 4: &lt;= 4000  |	$3500 USD                 |
| Livello 5: &lt;= 10000 |	$5000 USD                 |
{:caption="Tabella 6. Tabella prezzi di livello a blocchi" caption-side="top"}

La seguente tabella
illustra quanto paghi con un piano basato su un modello di prezzi di livello a blocchi:

| Quantità di elementi   | Calcolo dell'addebito                                                      | Prezzo totale|
|------------------|-------------------------------------------------------------------------|------------|
| 500              | Il numero di elementi rientra nel livello 1, quindi
il prezzo totale è $1000 USD. | $1000 USD  |
| 1500             | Il numero di elementi rientra nel livello 2, quindi
il prezzo totale è $1900 USD. | $1900 USD  |
| ...              | ...                                                                     | ...        |
| 5200             | Il numero di elementi rientra nel livello 5, quindi
il prezzo totale è $5000 USD. | $5000 USD  |
{:caption="Tabella 7. Calcolo dell'addebito utilizzando un modello di prezzi di livello a blocchi" caption-side="top"}
