# 🚀 MATHJS LAB: GUIDA AVANZATA (V2.0)

Benvenuto nel laboratorio di livello 2. Oggi scopriremo un segreto: i computer a volte "sbagliano" i calcoli con la virgola. Impareremo come correggerli usando la matematica delle frazioni e come gestire i numeri infiniti.

---

## 🟢 MODULO 1: IL "BUG" DELLA VIRGOLA

**Obiettivo:** Scoprire perché i computer faticano con i numeri decimali e come risolvere il problema.

### 1. L'errore invisibile

I computer ragionano in binario (solo 0 e 1). Alcuni numeri che per noi sono semplici (come 0.1) sono impossibili da scrivere perfettamente in binario, un po' come 1 diviso 3 (0.3 periodico).

**👉 PROVA ORA:**
Digita questo calcolo nella console:
`0.1 + 0.2`

* **Cosa succede:** Il risultato sarà `0.30000000000000004`.
* **Analisi:** Hai visto quel `4` alla fine? È un errore di arrotondamento digitale!

### 2. La Soluzione (Frazioni)

Per evitare questo errore, dobbiamo ordinare al computer di trattare i numeri come "pezzi interi" (frazioni) e non come decimali approssimati.

**👉 PROVA ORA:**
Digita questo comando:
`fraction(0.1) + fraction(0.2)`

* **Risultato atteso:** `0.3` (Perfetto ed esatto).

---

## 🟡 MODULO 2: NUMERI PERIODICI E RATIO

**Obiettivo:** Scrivere numeri con cifre infinite (periodici) e vederli come frazioni esatte.

### 3. La sintassi del Periodico

In matematica, sui quaderni, usiamo una barretta sopra il numero. Qui usiamo le parentesi tonde per indicare la parte che si ripete all'infinito.

* `0.33333...` si scrive **`0.(3)`**
* `0.285714...` si scrive **`0.(285714)`**

**👉 PROVA ORA:**
Digita:
`fraction('0.(3)')`

* **Risultato:** `1/3` (Il sistema ha riconosciuto il numero periodico!).

### 4. Visualizzare come "Ratio" (Rapporto)

Abbiamo potenziato la console con un comando speciale chiamato `printRatio`. Questo comando forza il computer a mostrarti la frazione invece del numero con la virgola.

**👉 PROVA ORA:**

1. Vuoi vedere cos'è 0.125 in frazione?
Scrivi: `printRatio(0.125)`  Risultato: `1/8`
2. Vuoi vedere il numero periodico 0,666...?
Scrivi: `printRatio(fraction('0.(6)'))`  Risultato: `2/3`

---

### 🧩 MICRO-SFIDA A: IL PASTICCERE PRECISO

Devi dividere 1 kg di impasto speciale in 3 parti esattamente uguali.
Se usi una calcolatrice normale e fai `1 / 3` ottieni `0.333`. Se poi rimoltiplichi i tre pezzi (`0.333 * 3`) ottieni `0.999`. Manca un grammo!

**Il tuo compito:**
Dimostra alla console che usando le frazioni puoi tornare esattamente a 1.

1. Crea la variabile "pezzo": `pezzo = fraction('1/3')`
2. Moltiplica per 3: `pezzo * 3`

*Se hai fatto tutto bene, il risultato sarà **1** tondo, senza virgole.*

---

## 🟠 MODULO 3: ALGEBRA E FORMATTAZIONE

**Obiettivo:** Convertire numeri "brutti" in frazioni eleganti e mischiare le operazioni.

### 5. Convertire Decimale in Frazione

Hai trovato un numero decimale strano, tipo `0.32`, e vuoi sapere a quale frazione corrisponde per semplificare un'equazione.

**👉 PROVA ORA:**
Digita:
`printRatio(0.32)`

* **Risultato:** `8/25`

### 6. Espressioni Miste

Puoi mischiare numeri normali, periodici e frazioni nella stessa riga. La console cercherà di mantenere la precisione massima.

**👉 PROVA ORA:**
Somma un numero periodico a un decimale semplice (0.5 è un mezzo):
`fraction('0.(3)') + 0.5`

* **Risultato:** Vedrai `0.8333...` ma accanto vedrai anche la frazione `5/6`.

---

### 🏆 CHALLENGE FINALE: IL RIPARATORE

Il computer di bordo segna un valore di energia pari a `0.142857142857...`.
Il manuale dice che il sistema è stabile solo se l'energia è pari a **1/7**.
Quel numero decimale corrisponde a 1/7?

**Comando per verificare:**
`printRatio(0.(142857))`

*Corrisponde?*
