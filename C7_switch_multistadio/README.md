# Switch Multistadio – Omega Network

Questo capitolo raccoglie gli esercizi sullo **switch multistadio**, sviluppati in **VHDL** e testati mediante simulazione.

## Esercizio 11 – Progettazione di uno switch multistadio

### Esercizio 11.1

* **Obiettivo**: Progettare e implementare uno switch multistadio secondo il modello **omega network**.
* **Caratteristiche**:

  * Scambio di messaggi di 2 bit ciascuno da un nodo sorgente a un nodo destinazione.
  * Rete composta da 4 nodi.
  * Implementazione di uno **schema a priorità fissa** tra i nodi (es. nodo 1 con priorità più alta, nodo 4 con priorità più bassa).
* **Implementazione**: Utilizzo di moduli VHDL per gestire lo switching e la priorità, con simulazioni per verificare il corretto instradamento dei messaggi.

---

**Nota**: Tutti i moduli e testbench sono contenuti nelle rispettive cartelle; questo README fornisce una panoramica generale dell’esercizio.
