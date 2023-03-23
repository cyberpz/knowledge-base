La maggior parte degli exchange hanno diversi tipi di ordine:
- Il limit
- Market
- Stop Limit / Stop Loss
- OCO

# Limite
Un **ordine limit** è un'istruzione per attendere che il prezzo raggiunga un prezzo limite o migliore, prima di essere eseguito.
Si compra / vende al prezzo indicato.
Se si imposta una quantità maggiore a quella disponibile nel book l'ordine viene eseguito parzialmente.
Nel caso si vuole comprare, e si inserisce un ordine al di sotto del prezzo corrente, 
l'ordine verra inserito al

---

# Mercato
Un **ordine market** è un'istruzione per acquistare o vendere immediatamente (al prezzo attuale del mercato).

---

# Stop Limit

Un [ordine stop-limit](https://academy.binance.com/it/articles/what-is-a-stop-limit-order) è un tipo di ordine per limitare le perdite che si possono verificare durante un trade. Questo tipo di ordine ti consente di impostare un prezzo di stop e un prezzo limite. Se BTC fosse scambiato a 10000€ e puoi impostare un ordine stop-limit a un prezzo stop di 9900€ e un prezzo limite di 9895€. Quindi verrà piazzato un ordine limit pari a 9985€ quando il prezzo scende di 10€.

Comunque tieni presente che l'ordine viene eseguito solo dopo che il prezzo di stop è stato raggiunto. Corri ancora il rischio che il prezzo non si riprenda, in questo caso non si ha una protezione se il prezzo continua a scendere sotto i 9985€ e allo stesso tempo l'ordine potrebbe non essere riempito.

---

# OCO (One Cancel Other)
Un ["un ordine cancella ordine" (OCO)](https://academy.binance.com/it/articles/what-is-an-oco-order) è uno strumento sofisticato che ti consente di combinare due ordini condizionali. Non appena uno dei due viene attivato, l'altro viene annullato. Se prendiamo l'esempio di _BTC a 10000€_, è possibile utilizzare un ordine OCO per acquistare Bitcoin quando il prezzo scende a 9900€ o per vendere quando il prezzo sale a 11000€. Uno dei due verrà eseguito per primo, di conseguenza il secondo verrà automaticamente annullato.

---

# Cos'è il time in force?

Un altro concetto importante da capire quando si parla di ordini è _il time in force_. Questo è un parametro che specifichi quando apri un trade, specificando le condizioni per la sua scadenza.

### Good-Til-Canceled (GTC)

Good-Til-Canceled (GTC) è un'istruzione che stabilisce che un trade deve essere tenuto aperto fino a quando non viene eseguito o annullato manualmente. Generalmente le piattaforme di trading di criptovalute utilizzano questa, come opzione predefinita. 

Nei mercati azionari, un'alternativa comune, consiste nel chiudere l'ordine a fine giornata di trading. Poiché il mercato crypto opera 24 ore su 24, l'opzione GTC è la più diffusa.

### Immediate-or-Cancel (IOC)

Gli ordini IOC (Immediate-or-Cancel) stabiliscono che qualsiasi parte di un ordine che non venga immediatamente eseguito deve essere annullato. Immaginiamo che tu inserisca un ordine per acquistare 10 BTC a 10000€, ma puoi ottenere solo 5 BTC a quel prezzo di esecuzione. In questo caso, acquisteresti quei 5 BTC, e il resto dell'ordine verrebbe cancellato.

### Fill-or-Kill (FOK)

Gli ordini Fill-or-Kill (FOK) vengono eseguiti immediatamente o in caso contrario vengono annullati (cancellati). Se hai inserito un ordine (FOK) con l'intento di acquistare 10 BTC al prezzo di 10000€, in questo caso l'ordine non verrà eseguito parzialmente. Se l'intero ordine di 10 BTC non è immediatamente disponibile a quel prezzo, verrà annullato.

---

# Cos'è un ordine Iceberg?

Una funzione opzionale che consente di acquistare o vendere una grande quantità di beni in quantità predeterminate più piccole al fine di nascondere la quantità totale dell'ordine.

In un ordine limit, per esempio, si inserisce nel campo iceberg la quantità che si vuole mostrare in book. 

> [!warning] Attenzione: per limitazione, un ordine iceberg puo essere diviso in massimo 10 parti. 
