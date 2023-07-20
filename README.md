# Derivati

# Opzioni finanziarie
Le opzioni vengono negoziate sia in borsa sia nei mercati over the counter. Esistono due tipi di 
opzioni: 
-Call, danno diritto al portatore di comprare un’attività entro una certa data per un certo 
prezzo 
-Put, danno il diritto al portatore di vendere un’attività entro una certa data per un certo 
prezzo. 
Il prezzo nel contratto è indicato come prezzo di base (strike price). 
Per schematizzare meglio le opzioni queste si possono suddividere in base alla data di esercizio: 
-Le opzioni europee sono quelle che possono essere esercitate solo alla scadenza 
-Le opzioni americane possono essere esercitate in qualsiasi momento e vengono scambiate 
in borsa.
Nelle opzioni il portatore ha il diritto di fare qualcosa ma non l’obbligo di esercitare questo diritto. 
Quanto appena indicato è la caratteristiche che distingue le opzioni da forward e futures nei quali 
ci si impegna a comprare o vendere l’attività sottostante ed inoltre non è previsto un costo per 
entrare mentre nelle opzioni vi è un premio da pagare.
Nel mercato delle opzioni vi sono diversi traders:
Compratori di call 
Venditori di call 
Compratori di puts 
Venditori di puts. 
Si osserva che i compratori hanno posizioni lunghe e i venditori hanno posizioni corte mentre il 
writer è colui che vende le opzioni.

## Tipi di traders
Vi sono tre tipologie di trader:
Gli headgers usano i derivati per ridurre i rischi che derivano dalle loro esposizioni nei 
confronti del mercato. Gli headgers si trovano a fronteggiar il rischio associato con il prezzo 
di un’attività per ridurre o eliminare questo rischio ricorrendo i derivati.
Gli speculatori usano i derivati per scommettere sull’evoluzione di prezzo.
Gli arbitraggisti assumono posizione di segno opposto su due o più contratti per ottenere 
profitto. In altri termini cercano di trarre vantaggio dalle differenze di prezzi di due diversi 
mercati. Ad esempio, se si accorgono che il prezzo futures di un’attività sta andando fuori 
linea rispetto al prezzo spot assumono posizioni di segno opposto nei due mercati per 
bloccare un profitto.

Le opzioni sono differenti rispetto ai derivati fino a ieri in quanto le opzioni danno a chi le detiene il 
diritto, ma non l’obbligo, di fare qualcosa mentre nel caso degli altri derivati le due parti sono 
impegnate a fare qualcosa.
La negoziazione dei forward e futures non costa nulla mentre l'acquisto di un'opzione richiede il
pagamento di un premio immediato. 

Come abbiamo visto esistono due tipologie di opzioni: 
Le call, che danno il diritto al possessore di comprare un’attività entro una determinata data 
con un certo prezzo
Le put, che danno il diritto al possessore di vendere una determinata attività entro una 
determinata data ad un certo prezzo. 
La data specifica del contratto è chiamata data di scadenza e il prezzo specificato nel contratto è
chiamato prezzo di esercizio. 
In ogni contratto sono presenti:
L’investitore che ha assunto una posizione lunga (ha acquistato l’opzione) chiamato anche 
holder 
L’investitore che ha assunto una posizione corta (venduto l’opzione) chiamato writer.

## Posizioni su opzioni e payoff
Bisogna osservare il funzionamento di un’opzione osservando il suo payoff sia per quanto riguarda 
l’holder che il writer, difatti di analizzeranno le relative posizioni su opzioni.
Bisogna introdurre alcune nozioni prendendo in considerazione:
-Un contratto di opzione che riguarda un’unità del bene sottostante (moltiplicando i singoli 
importi per il numero di titoli presenti all’interno del contratto). 
-x=prezzo di esercizio
-L’intervallo di tempo preso in considerazione è pari a [0, 𝑇] , questo intervallo indica il 
momento in cui comincia il contratto 0 e il momento in cui termina 𝑇
-Un generico istante 𝑡 che appartiene a [0, 𝑇]
-st= prezzo del sottostante in t
k= premio pagato da holder


## Guadagno opzioni call
Riprendendo quanto detto bisogna osservare che l’opzione a scadenza se:
st ≤ x , non verrà esercitata l’opzione e quindi si avrà una perdita pari a −𝐾
st > x allorà l’opzione verrà esercitata e il guadagno sarà pari a 𝑆𝑇 − 𝑋 − 𝐾
In termini matematici è possibile riscrivere il guadagno dell’holder nel seguente modo:

𝐺(𝑆𝑇) = (
−𝐾 ; 
𝑆𝑇 ≤ 𝑋
𝑆𝑇 − 𝑋 − 𝐾 ; 𝑆𝑇 > x )

![image](https://github.com/lreg8810/Derivati/assets/118115323/0efa3e0d-8d40-463b-95a1-6da25cb7ea42)

Quello che si osserva è che l’holder eserciterà l’opzione solo nel caso in cui 𝑆𝑇 > 𝑋 , dal punto di 
vista grafico la linea rossa rappresenta il guadagno che è negativo inizialmente ma poi diventa 
positivo, nel tratto rosa, facendo sì che il guadagno diventi una funzione lineare generando un 
guadagno positivo solo dopo che 𝑆𝑇 superi il valore 𝑋 + 𝐾.

## Guadagno opzioni put

![image](https://github.com/lreg8810/Derivati/assets/118115323/eecf0596-fb1a-4afe-a128-0675d47a7bd0)


In base al grafico la linea orizzontale verde rappresenta il punto in cui la funzione si spezza, e si 
osserva che se:
st> x l’holder perde il premio (freccia rossa)
st < x, la funzione è una funzione lineare con coefficiente angolare -1.
La seguente funzione lineare è bene che venga esercitata solo se 𝑆𝑇 < 𝑋, il guadagno sarà 
positivo solo se 𝑆𝑇 < 𝑋 − 𝐻 (punto rosa).

## Modello binomiale 

Nel contesto delle opzioni finanziarie, il modello binomiale è un metodo ampiamente utilizzato per valutare le opzioni europee. Le opzioni europee sono contratti finanziari che danno al possessore il diritto, ma non l'obbligo, di acquistare (opzione call) o vendere (opzione put) un'attività sottostante a un prezzo specifico (prezzo di esercizio) entro una data futura specifica (scadenza).

Il modello binomiale per le opzioni si basa su diverse assunzioni:
1. Il prezzo dell'attività sottostante può variare solo in modo discreto durante l'intervallo di tempo tra l'oggi e la scadenza dell'opzione. Di solito, si considerano due soli possibili risultati per il prezzo dell'attività sottostante: salire o scendere.
2. Gli incrementi di prezzo dell'attività sottostante sono costanti e noti.
3. Non ci sono costi di transazione, né commissioni o spese.
4. Non ci sono opportunità di arbitraggio senza rischio nei mercati.

Sotto queste assunzioni, il modello binomiale costruisce un albero binomiale che rappresenta tutti i possibili scenari di prezzo dell'attività sottostante. In ogni nodo dell'albero, si calcola il valore dell'opzione in base al prezzo dell'attività sottostante in quel nodo e alle probabilità associate ai rami (probabilità di salire o scendere). Si risale l'albero, calcolando i valori delle opzioni a partire dalla scadenza e arrivando all'oggi.

Il prezzo dell'opzione al giorno odierno (prezzo del giorno zero o prezzo iniziale) è il valore stimato dell'opzione in quel momento, e rappresenta il prezzo al quale il possessore dell'opzione può decidere di esercitare il diritto di acquisto o vendita.

Una delle formule chiave utilizzate nel modello binomiale per calcolare il valore dell'opzione è la seguente:

```
V_t = max(0, p * V_u + (1 - p) * V_d) / (1 + r)
```

Dove:
'V_t' è il valore dell'opzione al nodo corrente.
'V_u' è il valore dell'opzione al nodo successivo in caso di aumento del prezzo dell'attività sottostante.
'V_d' è il valore dell'opzione al nodo successivo in caso di diminuzione del prezzo dell'attività sottostante.
'p' è la probabilità di un aumento del prezzo dell'attività sottostante.
'1 - p' è la probabilità di una diminuzione del prezzo dell'attività sottostante.
'r' è il tasso di interesse senza rischio per l'intervallo di tempo considerato.

Ripetendo questo processo per tutti i nodi dell'albero binomiale, è possibile ottenere il valore dell'opzione al giorno zero, ovvero il suo prezzo attuale nel mercato.

## Modello di Black-Sholes

Il modello di Black-Scholes è una formula matematica utilizzata per stimare il prezzo di un'opzione europea (sia call che put) sul mercato finanziario. La formula prende il nome dai suoi creatori, Fischer Black, Myron Scholes e Robert Merton, ed è stata pubblicata per la prima volta nel 1973.

Il modello di Black-Scholes si basa su alcune importanti assunzioni e considerazioni:

1. Mercato efficiente: Si assume che i mercati siano efficienti, il che significa che non ci sono opportunità di arbitraggio senza rischio.

2. Assenza di costi di transazione: Non ci sono costi di transazione o commissioni nelle negoziazioni.

3. Assenza di dividendi: L'attività sottostante non emette dividendi durante la vita dell'opzione.

4. Movimenti dei prezzi dell'attività sottostante: Si considera che il prezzo dell'attività sottostante segua un processo stocastico geometrico di tipo Browniano.

La formula di Black-Scholes per il prezzo di un'opzione call è:

```
c = S * N(d1) - X * e^(-r * T) * N(d2)
```

Dove:
- `c` è il prezzo dell'opzione call.
- `S` è il prezzo corrente dell'attività sottostante (ad esempio, azione, indice, ecc.).
- `N(d1)` è la funzione cumulativa della distribuzione normale standard calcolata utilizzando il valore `d1`.
- `N(d2)` è la funzione cumulativa della distribuzione normale standard calcolata utilizzando il valore `d2`.
- `X` è il prezzo di esercizio (strike price) dell'opzione.
- `r` è il tasso di interesse senza rischio per l'intervallo di tempo fino alla scadenza dell'opzione.
- `T` è il tempo rimanente fino alla scadenza dell'opzione, espresso in anni.
- `e` è la costante di Nepero (circa 2.71828), base del logaritmo naturale.

I valori `d1` e `d2` sono calcolati come segue:

```
d1 = (ln(S / X) + (r + (σ^2) / 2) * T) / (σ * sqrt(T))
d2 = d1 - σ * sqrt(T)
```

Dove:
- `ln` è il logaritmo naturale.
- `σ` rappresenta la volatilità del prezzo dell'attività sottostante, ovvero la deviazione standard del rendimento dell'attività sottostante.
- `sqrt(T)` è la radice quadrata del tempo fino alla scadenza.

# Futures e Forward

Forward Contract:

Il forward contract (contratto forward) è un accordo personalizzato tra due parti per acquistare o vendere un bene o un'attività finanziaria in futuro a un prezzo specifico concordato al momento della stipula del contratto. Questi contratti sono negoziati privatamente tra le parti coinvolte, spesso tramite banche o istituzioni finanziarie. I principali punti da considerare riguardo ai contratti forward sono:

Personalizzazione: Poiché i contratti forward sono negoziati privatamente, le loro specifiche, come la dimensione del contratto, la data di scadenza e il prezzo concordato, possono essere personalizzate per soddisfare le esigenze specifiche delle parti coinvolte.

Mercato OTC: Il mercato dei contratti forward è noto come mercato over-the-counter (OTC), il che significa che le negoziazioni avvengono al di fuori di un'entità regolamentata.

Rischi di controparte: Nel contratto forward, c'è un rischio di controparte, il che significa che se una delle parti non adempie ai propri obblighi contrattuali, l'altra parte potrebbe incorrere in perdite.

Futures Contract:

Il futures contract (contratto futures) è simile al contratto forward nel senso che rappresenta un accordo per acquistare o vendere un bene o un'attività finanziaria in futuro a un prezzo specifico concordato. Tuttavia, ci sono alcune caratteristiche che rendono i contratti futures diversi dai contratti forward:

Standardizzazione: I contratti futures sono altamente standardizzati, il che significa che hanno dimensioni, date di scadenza e specifiche standardizzate che sono stabilite dalla borsa su cui vengono negoziati.

Mercato Organizzato: I contratti futures vengono negoziati in borse regolamentate, come il Chicago Mercantile Exchange (CME) o l'Intercontinental Exchange (ICE), che fungono da intermediari per le transazioni.

Liquidità: Grazie alla loro standardizzazione e alla negoziazione su borse regolamentate, i contratti futures sono generalmente più liquidi dei contratti forward.

Sistema di Marginazione: Nei contratti futures, i partecipanti devono fornire un margine iniziale come garanzia per coprire eventuali perdite future. Inoltre, il valore della posizione viene valutato giornalmente tramite marking to market, e gli aggiustamenti del margine vengono fatti se necessario.

Rischi di Controparte Ridotti: A causa del sistema di margine e della regolamentazione delle borse, i rischi di controparte sono ridotti nei contratti futures.

In sintesi, mentre sia i contratti forward che i contratti futures permettono agli investitori di coprire il rischio o speculare sui movimenti dei prezzi in futuro, i contratti futures sono più standardizzati, negoziati su borse regolamentate, e presentano un sistema di margine e liquidazione giornaliera, il che li rende più accessibili e convenienti per molti partecipanti al mercato rispetto ai contratti forward personalizzati e negoziati privatamente.

## calcolo del prezzo forward o prezzo dei futures
Per il calcolo del prezzo forward o prezzo dei futures (F0) sulla base del prezzo spot corrente dell'attività sottostante (S0), il tasso di interesse privo di rischio (r) e la scadenza del contratto in anni (T). La formula è espressa come:

F0 = S0 × e^(r⋅T)

Dove:

F0 è il prezzo forward o prezzo dei futures. S0 è il prezzo spot corrente dell'attività sottostante. e è la base del logaritmo naturale (costante di Nepero, approssimativamente 2.71828). r è il tasso di interesse privo di rischio. T è la scadenza del contratto espressa in anni.


## Valore dei contratti
I forward quando vengono negoziati hanno un valore nullo e successivamente potranno avere un valore positivo o negativo e adottando la metodologia vista in precedenza si osservi che:

𝑓 = (𝐹0 − 𝑋) ∗ 𝑒^(−𝑟𝑇)

dove:

𝑓 rappresenta il valore corrente della posizione lunga del contratto forward con prezzo di consegna 𝑋.

𝐹0 è il prezzo forward negoziato inizialmente, che viene posto uguale al prezzo di consegna 𝑋 al momento della negoziazione del contratto.

𝑋 è il prezzo di consegna del contratto forward, che rimane inalterato nel tempo.

𝑟 è il tasso di interesse privo di rischio valido per la scadenza del contratto.

𝑇 è il periodo di tempo fino alla scadenza del contratto, espresso in anni.

L'equazione descrive come il valore della posizione lunga (f) cambia nel tempo in base alle variazioni del prezzo forward (F0) rispetto al prezzo di consegna (X) e al tasso di interesse (r).

Quando il prezzo futures cambia, il guadagno/perdita sui futures viene calcolato ∆𝑝𝑟𝑒𝑧𝑧𝑜 ∗ 𝑑𝑖𝑚𝑒𝑛𝑠𝑖𝑜𝑛𝑒 𝑑𝑒𝑙 𝑐𝑜𝑛𝑡𝑟𝑎𝑡𝑡𝑜 Il guadagno/perdita vengono contabilizzati immediatamente dato che i futures vengono liquidati giornalmente

## marking to market
Il "marking to market"  della clearing house è un processo critico utilizzato per valutare e regolare le posizioni dei partecipanti ai mercati finanziari, in particolare nei contratti futures e opzioni. Una clearing house è un'entità che agisce come intermediario tra le parti coinvolte in tali contratti, fornendo servizi di compensazione e garanzia, svolge le seguenti funzioni:

1. **Valutazione giornaliera delle posizioni:** Ogni giorno, la clearing house valuta il valore corrente delle posizioni di ciascun partecipante in base ai prezzi di mercato correnti. Questo prezzo di mercato è noto come "prezzo di liquidazione" o "prezzo di chiusura".

2. **Regolazione dei margini:** Dopo aver valutato le posizioni, la clearing house aggiorna i margini richiesti dai partecipanti. Il margine è un deposito iniziale richiesto per garantire l'adempimento degli obblighi contrattuali e coprire eventuali perdite future. La clearing house può richiedere ai partecipanti di fornire ulteriori fondi (chiamati "margine aggiuntivo" o "margine di variazione") se il valore delle loro posizioni scende al di sotto dei livelli minimi richiesti.

3. **Liquidazione delle perdite e dei guadagni:** Se una posizione subisce perdite, il partecipante deve fornire i fondi necessari per coprire tali perdite. D'altra parte, se una posizione guadagna, i profitti vengono accreditati sul conto del partecipante. Questo processo di regolazione giornaliera continua finché la posizione non viene chiusa o scade.

4. **Riduzione del rischio di controparte:** La clearing house agisce come controparte centrale per tutti i partecipanti, riducendo il rischio di controparte. Se un partecipante non adempie ai propri obblighi, la clearing house assume la responsabilità dell'adempimento e si assicura che gli altri partecipanti non subiscano perdite significative.

5. **Garanzia dell'integrità del mercato:** Il processo di marking to market aiuta a mantenere l'integrità del mercato finanziario, garantendo che tutte le parti rispettino gli obblighi contrattuali e fornendo trasparenza nei valori delle posizioni.



