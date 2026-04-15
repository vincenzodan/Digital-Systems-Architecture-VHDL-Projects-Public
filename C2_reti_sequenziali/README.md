# Reti Sequenziali Elementari

Questo capitolo raccoglie gli esercizi sulle **reti sequenziali elementari**, sviluppati in **VHDL** e testati mediante simulazione, con implementazione su board FPGA quando previsto.

## Esercizio 3 – Riconoscitore di sequenze

### Esercizio 3.1

* **Obiettivo**: Progettare una macchina che riconosca la sequenza 101.
* **Ingressi/uscite**: segnale binario `i`, segnale di tempificazione `A`, segnale di modo `M`; uscita `Y` alta quando la sequenza è riconosciuta.
* **Funzionamento**:

  * `M = 0`: valutazione dei bit in gruppi di 3 (sequenze non sovrapposte).
  * `M = 1`: valutazione bit per bit, sequenze parzialmente sovrapposte.

### Esercizio 3.2

* **Obiettivo**: Sintetizzare e implementare la macchina su board.
* **I/O Board**: Switch `S1` per input `i`, switch `S2` per modo `M`, bottoni `B1` e `B2` per acquisizione sincrona con il segnale di tempificazione `A`, LED per output `Y`.

## Esercizio 4 – Shift Register

### Esercizio 4.1

* **Obiettivo**: Progettare un registro a scorrimento di N bit con shift a destra o sinistra di 1 o 2 posizioni.
* **Caratteristiche**: Implementazione sia comportamentale che strutturale, con generic per numero di bit e segnali di selezione per modalità di funzionamento.

## Esercizio 5 – Cronometro

### Esercizio 5.1

* **Obiettivo**: Progettare un cronometro che scandisca secondi, minuti e ore a partire da un clock prefissato.
* **Funzionalità**: Ingresso `set` per inizializzazione, ingresso `reset` per azzerare il tempo, implementazione strutturale con contatori.

### Esercizio 5.2

* **Obiettivo**: Sintetizzare e implementare su board.
* **I/O Board**: Display a 7 segmenti per visualizzazione, switch per orario iniziale, bottoni per set e reset.

### Esercizio 5.3

* **Obiettivo**: Estendere il cronometro per memorizzare fino a N intertempi, visualizzabili tramite pressione di un bottone.

## Esercizio 6 – Sistema PO_PC

### Esercizio 6.1

* **Obiettivo**: Progettare un sistema con ROM di N locazioni da 8 bit, macchina combinatoria M (8 bit in input, 4 bit in output) e memoria MEM di N locazioni.
* **Funzionamento**: Avvio con segnale `START`, controllo della tempificazione, lettura sequenziale ROM, trasformazione con M, scrittura in MEM, indirizzi forniti da contatore, lettura e scrittura sincrona.

### Esercizio 6.2

* **Obiettivo**: Sintetizzare e implementare su board.
* **I/O Board**: Due bottoni per read e reset, LED per visualizzazione delle uscite della macchina istante per istante.

---

**Nota**: Tutti i moduli e i testbench si trovano nelle rispettive cartelle; questo README fornisce una panoramica generale degli esercizi.
