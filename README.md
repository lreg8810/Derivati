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
−𝐾 ; 
𝑆𝑇 ≤ 𝑋
𝑆𝑇 − 𝑋 − 𝐾 ; 𝑆𝑇 > x )

![image](https://github.com/lreg8810/Derivati/assets/118115323/0efa3e0d-8d40-463b-95a1-6da25cb7ea42)








