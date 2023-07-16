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


## Guadagno dell’holder nella call
Riprendendo quanto detto bisogna osservare che l’opzione a scadenza se:
st ≤ x , non verrà esercitata l’opzione e quindi si avrà una perdita pari a −𝐾
st > x allorà l’opzione verrà esercitata e il guadagno sarà pari a 𝑆𝑇 − 𝑋 − 𝐾
In termini matematici è possibile riscrivere il guadagno dell’holder nel seguente modo:

𝐺(𝑆𝑇) = (
−𝐾 ; 𝑆𝑇 ≤ 𝑋
𝑆𝑇 − 𝑋 − 𝐾 ; 𝑆𝑇 > x )

![image](https://github.com/lreg8810/Derivati/assets/118115323/0efa3e0d-8d40-463b-95a1-6da25cb7ea42)


Quello che si osserva è che l’holder eserciterà l’opzione solo nel caso in cui 𝑆𝑇 > 𝑋 , dal punto di 
vista grafico la linea rossa rappresenta il guadagno che è negativo inizialmente ma poi diventa 
positivo, nel tratto rosa, facendo sì che il guadagno diventi una funzione lineare generando un 
guadagno positivo solo dopo che 𝑆𝑇 superi il valore 𝑋 + 𝐾. 
Analizzando la posizione del writer si osserva che: 
 Qualora l’holder non esercitasse l’opzione il writer incasserà il premio, linea verde.
 Nel momento in cui 𝑆𝑇 𝑠𝑢𝑝𝑒𝑟𝑎 𝑋 l’holder è chiamato a esercitare e il wiriter perdere tanto 
più quanto 𝑆𝑇 è grande e quindi illimitata (tratto giallo).
Nello specifico possiamo osservare come: 
 L’holder avrà un guadagno illimitato ma una perdita limitata 
 Il writer avrà un guadagno limitato e una perdita illimitata, ovviamente esso dovrà coprire la 
posizione assunta per evitare perdite. 
14
Dato che si analizzano delle cifre di denaro in istanti di tempo differenti per ovviare a tale 
problematica allora è necessario, dal punto di vista finanziario, riscrivere il guadagno, 𝐺′ , utilizzando 
un tasso 𝑖, ovvero:
𝐺
′(𝑆𝑇) = {
−𝐾 (1 + 𝑖𝑇); 𝑆𝑇 ≤ 𝑋
𝑆𝑇 − 𝑋 − 𝐾(1 + 𝑖𝑇); 𝑆𝑇 > 𝑋
La differenza che intercorre tra 𝐺
′𝑒 𝐺 è che in 𝐺
′
si tiene in considerazione dello scarto temporale 
che intercorre tra 0 𝑒 𝑇.
Scadenza nel put e guadagno
Nel put il guadagno sé dato da:
𝐺(𝑆𝑇) = {
𝑋 − 𝑆𝑇 − 𝐻 ; 𝑆𝑇 < 𝑋
−𝐻; 𝑆𝑇 ≥ 𝑋
L’holder di un put può vendere a 𝑋 quello che sul mercato venderebbe a 𝑆𝑇 , quindi la vendita diretta 
sul mercato è vantaggiosa rispetto a quella prevista dall’opzione e quindi se:
 𝑆𝑇 ≥ 𝑋 , l’holder è costretto ad abbandonare il contratto perdendo il premio che per 
distinguerlo dalla call viene indicato con H
 𝑆𝑇 < 𝑋 , l’holder eserciterà l’opzione ottenendo il guadagno 𝑋 − 𝑆𝑇 − 𝐻
La rappresentazione grafica del put è la seguente:

![image](https://github.com/lreg8810/Derivati/assets/118115323/6406e299-be35-47c4-ac2a-b0eb413fd921)

In base al grafico la linea orizzontale verde rappresenta il punto in cui la funzione si spezza, e si 
osserva che se:
 𝑆𝑇 > 𝑋 l’holder perde il premio (freccia rossa)
 𝑆𝑇 < 𝑋 , la funzione è una funzione lineare con coefficiente angolare -1.
La seguente funzione lineare è bene che venga esercitata solo se 𝑆𝑇 < 𝑋, il guadagno sarà 
positivo solo se 𝑆𝑇 < 𝑋 − 𝐻 (punto rosa).
Nel caso del put
 L’holder avrà un guadagno limitato ed anche una perdita. 
15
 Il writer avrà una perdita limitata con un guadagno limitato. 
Anche per il put è possibile introdurre la notazione introdotta in precedenza per confrontare il valore 
di 𝑆𝑡 , con 0 < 𝑡 < 𝑇, confrontandolo con il valore 𝑋 , allora in questo caso la situazione è speculare 
rispetto a prima e quindi: 
 𝑆𝑇 < 𝑋 , ci si trova in una situazione in the money in quanto il put mi dà la possibilità di 
vendere a X quello che sul mercato venderei a meno.
 𝑆𝑇 = 𝑋 at the money 
 𝑆𝑇 > 𝑋 out of the money







