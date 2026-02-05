# Guida Studente 

Questa guida è divisa in piccoli passi ("Step"). 
- Leggi il concetto
- Guarda l'esempio
- Prova sulla console.

# 🚀 MathJS Lab

Useremo una console per risolvere o verificare problemi matematici scrivendo istruzioni precise.

## 🟢 Modulo 1: Primi Passi

**Obiettivo:** Usare la console come una calcolatrice smart.

### Step 1: Operazioni Base

Possiamo usare i simboli classici della tastiera.

* `+` Più
* `-` Meno
* `*` Per (asterisco)
* `/` Diviso (slash)
* `^` Potenza (caret: si trova sopra la "ì" sulla tastiera, in genere)

_Esempio: 
- Hai studiato oggi?
- Eh, `+` o `-` ..._

**👉 Prova:**

http://salvatorecapolupo.github.io/mathjs

Scrivi nella console `12 * 3` e premi Invio.
Scrivi `2 ^ 3` (due alla terza) e premi Invio.
Deve uscire 8. Prova a cambiare base ed esponente. 
Ricorda che questa sintassi funziona SOLO se importi Math.js, _non in generale._

### Step 2: L'ordine conta (Parentesi)

La console esegue prima le moltiplicazioni. Se vuoi fare prima un'addizione, devi "proteggerla" con le parentesi tonde `( )`.

**👉 Prova ora:**
Scrivi `2 + 3 * 4` (Risultato atteso: 14)
Scrivi `(2 + 3) * 4` (Risultato atteso: 20)

---

### 🧩 Micro-Sfida: Lo Scontrino

Hai trovato 50 euro (che fortuna). Decidi di comprare 2 videogiochi da 15 euro e un cavo da 5 euro.
Scrivi **una sola riga** di codice per calcolare il resto.

*Suggerimento:* `50 - (... calcolo della spesa ...)`

---

## 🟡 Modulo 2: Le Frazioni (Fractions)

**Obiettivo:** Evitare i numeri con la virgola infiniti (come 0.33333..., che abbiamo visto in IEEE 754) e lavorare con precisione differente.

### Step 3: Come creare una frazione

Il computer trasforma tutto in decimali, per cui non lavora con le frazioni. 
Grazie a Math.js possiamo superare questo limite. 
Per forzare a usare le frazioni, usiamo il comando `fraction`.
La sintassi è: `fraction(numeratore, denominatore)`.

**👉 Prova:**
Scrivi `fraction(1, 4)`
La console risponderà `1/4`.

### Step 4: Sommare le frazioni

Questo è il vero superpotere. Non serve fare il minimo comune multiplo a mente.

**👉 Prova ora:**
Vogliamo sommare un terzo e un sesto.
Scrivi: `fraction(1, 3) + fraction(1, 6)`
Risultato atteso: `0.5` (ovvero un mezzo).

---

### 🧩 Micro-Sfida B: La Torta

Siete in 4 amici. Ordinate 2 torte identiche.

1. Calcola quanta torta spetta a ciascuno usando `fraction`.
2. Un amico ti regala la sua parte. Somma la tua parte e la sua.
Quanto hai in totale?

*Comando:* `fraction(2, 4) + fraction(2, 4)`

---

## 🟠 Modulo 3: Memoria e Variabili (Expressions)

**Obiettivo:** Dare un nome ai numeri per non doverli riscrivere e risolvere problemi "generali".

### Step 5: Assegnare un nome

Usiamo l'uguale `=` per salvare un numero dentro una parola.

**👉 Prova ora:**
Scrivi `base = 10`
Scrivi `altezza = 5`
Ora la console ricorda questi valori.

### Step 6: Calcolare con le parole

Ora possiamo calcolare l'area usando i nomi che abbiamo appena inventato.

**👉 Prova ora:**
Scrivi `area = (base * altezza) / 2`
La console ti darà il risultato (25).
Se ora scrivi `base = 20` e rilanci il calcolo dell'area, il risultato si aggiornerà!

---

### 🧩 Micro-Sfida C: Il Viaggio (Fisica)

Dobbiamo calcolare il tempo di un viaggio. Formula: Tempo = Spazio / Velocità.

1. Crea una variabile `km` e metti valore 300.
2. Crea una variabile `vel` (velocità) e metti valore 100.
3. Scrivi la formula `km / vel` per trovare le ore.

---

## 🔴 Modulo 4: Algebra Simbolica

**Obiettivo:** Manipolare le lettere (x, y) per semplificare le espressioni dei compiti di matematica.

### Step 7: Il comando Simplify

Qui la console fa i compiti al posto tuo. Usa il comando `simplify('...')`.
**IMPORTANTE:** Devi mettere l'espressione tra virgolette semplici `' '` altrimenti la console cercherà il valore numerico di x.

**👉 Prova ora:**
Hai l'espressione: 2x + 3x
Scrivi: `simplify('2x + 3x')`
Risultato: `5 * x`

### Step 8: Prodotti notevoli e parentesi

Vediamo se la console riesce a sviluppare i calcoli complessi.

**👉 Prova ora:**
Vogliamo calcolare: 3 che moltiplica (x - 2) più 6.
Scrivi: `simplify('3 * (x - 2) + 6')`
Risultato atteso: `3 * x` (Ha fatto tutti i passaggi da sola!).

---

### 🧩 Micro-Sfida D: Il Quadrato del Binomio

Verifica se ti ricordi la formula del quadrato del binomio: (x + 3) alla seconda.

1. Prova a scriverlo su un foglio. Secondo te quanto fa?
2. Chiedilo alla console scrivendo:
`simplify('(x + 3) ^ 2')`
*(Nota: Potrebbe darti il risultato sviluppato o fattorizzato, prova a confrontarlo!)*

---
