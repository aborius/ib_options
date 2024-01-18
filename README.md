# Trading di Opzioni con Interactive Brokers
Questo progetto presenta un bot di trading di opzioni progettato per eseguire operazioni automatizzate sulla piattaforma Interactive Brokers (IB). L'obiettivo principale del bot è il trading di opzioni legate all'ETF SPY (S&P 500).

## Concetti Principali
Le opzioni sono contratti finanziari derivati che conferiscono il diritto, ma non l'obbligo, di acquistare (CALL) o vendere (PUT) un sottostante (ad esempio, un'azione, indice o valuta) a un prezzo specifico entro un determinato periodo di tempo. Il bot si concentra su opzioni legate all'ETF SPY.

## Funzionalità Principali
- Connessione a Interactive Brokers: Il bot si connette a Interactive Brokers per l'esecuzione delle operazioni di trading.
- Backfilling dei Dati: Inizialmente, il bot recupera i dati storici necessari per l'analisi.
- Aggiornamento Catene di Opzioni: Le catene di opzioni vengono aggiornate regolarmente per mantenere informazioni aggiornate sulle opzioni disponibili.
- Strategia di Trading: Il bot implementa una strategia basata su 3 chiusure consecutive più alte in un intervallo di 5 minuti, decidendo di acquistare contratti CALL fuori dal denaro con uno strike price più alto di $5.
- Gestione del Trade: Una volta iniziato un trade, il bot monitora le chiusure successive per decidere se vendere per ottenere un profitto.
