# Reti Combinatorie Elementari

Questo capitolo raccoglie gli esercizi sulle **reti combinatorie elementari** sviluppati in **VHDL** e testati mediante simulazione e, quando previsto, implementati su board FPGA Nexys A7.

## Esercizio 1 – Rete di interconnessione 16:4

### Esercizio 1.1

* **Obiettivo**: Progettare un multiplexer indirizzabile 16:1 utilizzando blocchi 4:1 preesistenti.
* **Approccio**: Architettura strutturale a due livelli, con 4 multiplexer 4:1 nel primo livello e un multiplexer 4:1 nel secondo livello.
* **Simulazione**: Verifica del corretto funzionamento con tutte le combinazioni di selezione.

### Esercizio 1.2

* **Obiettivo**: Creare una rete di interconnessione a 16 sorgenti e 4 destinazioni, combinando un multiplexer 16:1 e un demultiplexer 1:4.
* **Selezione**: `selm` (4 bit) per sorgente, `seld` (2 bit) per destinazione.
* **Simulazione**: Testbench dedicato per verificare che l’uscita corrisponda sempre alla sorgente e destinazione selezionate.

### Esercizio 1.3

* **Obiettivo**: Sintetizzare e implementare la rete di interconnessione su board.
* **I/O Board**: Switch per input (16 bit in due metà), LED per output (4 bit), rete di controllo con due bottoni per caricare i dati.

## Esercizio 2 – Sistema ROM+M

### Esercizio 2.1

* **Obiettivo**: Progettare un sistema combinatorio S composto da una ROM di 16 locazioni da 8 bit e una macchina combinatoria M.
* **Funzionamento**: Data l’entrata di 4 bit A, il sistema restituisce il valore della ROM all’indirizzo A trasformato dalla macchina M.
* **Vincolo**: La macchina M prende in ingresso 8 bit e restituisce 4 bit in uscita; il comportamento interno è a scelta dello studente.

### Esercizio 2.2

* **Obiettivo**: Sintetizzare e implementare il sistema ROM+M su board.
* **I/O Board**: Switch per selezionare l’indirizzo ROM, LED per visualizzare i 4 bit di output.

---

**Nota**: Tutti i moduli e i testbench sono contenuti nelle relative cartelle; il README è solo a scopo descrittivo e di riferimento rapido.

