# Le candele

> ![info|20](https://icons.iconarchive.com/icons/danrabbit/elementary/72/Button-info-icon.png) ATTENZIONE 
>Aggiungerò vocaboli in inglese, per rendere comuni termici tecnici. Non serve sapere l'inglese, ma vi faranno comodo saperli in futuro.

Le candele sono una rappresentazione grafica della variazione del prezzo nel frangente di tempo considerato.

## Com'è composta una candela?
Qualsiasi candela ha 4 valori fondamentali:

ITA | ENG | Abbreviato
Massimo | High | Max
Minimo | Low | Min 
Apertura | Open | O
Chiusura | Close | C

1. Il **massimo** è il valore più alto nella candela in considerazione.
2. Il **minimo** è quindi il valore più basso nello stesso frangente di tempo considerato.
3. L'**apertura** è il primo valore di prezzo allo scattare del minuto/ora/giorno ecc.. (per esempio nella candela di un minuto l'apertura viene fissata dal primissimo secondo -> :00)
4. La **chiusura** è l'ultimo valore di prezzo allo scattare del minuto/ora/giorno ecc.. (per esempio nella candela di un minuto l'apertura viene fissata dal primissimo secondo -> :59)

Non so che tipo di Yankee candle avete immaginato fin'ora, 
ma con un quadrato e due linee si costruisce una candela, come nell'immagine che viene, che descrive quindi i valori appena descritti.

![[Pasted image 20230213161845.png]]

In questa immagine, abbiamo due candele, 
La candela nera, perche è nera? 
1 minuto per pensare.

*Suggerimento*: Apertura e chiusura.


> Colori
è indifferente il colore che diamo alle candele, solitamente usiamo il rosso e il verde per tradizione, ma sono totalmente a vostra scelta.
Il Verde indica per tradizione la crescita.
Il Rosso indica per tradizione la decrescita.

Nel nostro caso la prima candela nera, è decrescente, quindi potrebbe essere anche rossa, per rendere meglio l'idea.

Ma come il computer a determinare se una candela cresce o decresce? e quindi dare il colore appropriato?  

Dipende se l'apertura è minore o maggiore rispetto alla chiusura:
- Verde-crescente: se Chiusura > Apertura
- Rosso-decrescente: se Apertura > Chiusura 

> INFO - Riassumendo
> Quindi i valori che determinano la candela sono:
> - apertura
> - chiusura
> - massimo 
> - minimo
> - durata in minuti/ore/giorni


# Frangente di tempo - TF
Il frangente di tempo considerato?
Si, perche la candela puo assumere i seguenti valori temporali: 
- 1, 3, 5, 15, 30 min 
- 1, 2, 4, 6, 8, 12 ore (Hour)
- 1 giorno (Day)
- 1 settimana (Week)
- 1 mese (Month)
- 
In inglese, frangente di tempo = timeframe, 
accorciato poi come TF.

In gergo, si parla per esempio di TF1, per dire che sto guardando il grafico con candele da 1 minuto, 
alla stessa maniera TF5 o TF1D saranno candele rispettivamente di 5minuti o 1giorno 

Ragionando per esempi, in sostanza una candela vale 5 minuti.
E quindi ogni 5 minuti, nasce una nuova candela, nel grafico.

Vediamo come cazz di vedono le candele in un [[3 - Grafico]]
