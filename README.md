🚀 MathJS Lab: Guida Avanzata
Benvenuto nel laboratorio 2.0. Oggi scopriremo che i computer a volte "sbagliano" i calcoli e come usare le frazioni per correggerli.

🟢 Modulo 1: Il "Bug" della Virgola
Obiettivo: Scoprire perché i computer faticano con i numeri decimali.

Step 1: L'errore invisibile
I computer ragionano in binario (0 e 1). Alcuni numeri semplici per noi (come 0.1) sono impossibili da scrivere perfettamente in binario.

👉 Prova ora: Scrivi: 0.1 + 0.2 Risultato atteso: 0.30000000000000004 Hai visto? Quel 4 alla fine è un errore di arrotondamento!

Step 2: La Soluzione (Frazioni)
Per evitare questo errore, dobbiamo dire al computer di trattare i numeri come "pezzi interi" (frazioni) e non come virgole.

👉 Prova ora: Scrivi: fraction(0.1) + fraction(0.2) Risultato atteso: 0.3 (Perfetto!)

🟡 Modulo 2: Numeri Periodici e Ratio
Obiettivo: Scrivere numeri con cifre infinite (periodici) e vederli come frazioni.

Step 3: La sintassi del Periodico
In matematica usiamo una barretta sopra il numero. Qui usiamo le parentesi tonde per indicare la parte che si ripete.

0.33333... si scrive 0.(3)

0.285714285714... si scrive 0.(285714)

👉 Prova ora: Scrivi: fraction('0.(3)') Risultato: 1/3

Step 4: Visualizzare come "Ratio" (Rapporto)
Abbiamo creato una funzione speciale chiamata printRatio che forza il computer a mostrarti la frazione invece del numero decimale.

👉 Prova ora:

Scrivi: printRatio(0.125) -> Vedrai 1/8

Scrivi: printRatio(fraction('0.(6)')) -> Vedrai 2/3

🧩 Micro-Sfida A: Il Pasticcere Preciso
Devi dividere 1 kg di impasto in 3 parti esatte. Se usi la calcolatrice normale fai 1 / 3 e ottieni 0.333.... Se poi moltiplichi per 3, ottieni 0.999... (manca un pezzetto!).

Compito: Dimostra che usando le frazioni torni esattamente a 1.

Crea la parte: pezzo = fraction('1/3')

Moltiplica per 3: pezzo * 3 Il risultato deve essere 1 tondo.

🟠 Modulo 3: Algebra e Formattazione
Obiettivo: Vedere i numeri in modi diversi.

Step 5: Convertire Decimale in Frazione
Hai un numero brutto, tipo 0.32. Vuoi sapere che frazione è.

👉 Prova ora: Scrivi: printRatio(0.32) Risultato: 8/25

Step 6: Espressioni Miste
Puoi mischiare tutto insieme.

👉 Prova ora: Somma un numero periodico e un decimale normale. Scrivi: fraction('0.(3)') + 0.5 Nota: Il sistema proverà a darti la risposta più precisa possibile (spesso una frazione).

Output Ibrido: Quando l'utente preme invio, la console ora controlla se il risultato è una frazione. Se lo è, mostra sia il valore decimale che la frazione (es. = 0.333... (1/3)), per aiutare i ragazzi a collegare i due concetti.
