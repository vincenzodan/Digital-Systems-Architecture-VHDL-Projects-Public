# Comunicazione con Handshaking

Questo capitolo raccoglie gli esercizi sul protocollo di **comunicazione con handshaking**, sviluppati in **VHDL** e testati mediante simulazione.

## Esercizio 8 – Sistema a due nodi

### Esercizio 8.1

* **Obiettivo**: Progettare un sistema composto da due nodi, A e B, che comunicano tramite handshaking.
* **Funzionamento**:

  * Entrambi i nodi possiedono una memoria interna con N stringhe di M bit, denominate X(i) per A e Y(i) per B.
  * Il nodo A trasmette ciascuna stringa X(i) a B mediante il protocollo di handshaking.
  * Il nodo B, ricevuta la stringa X(i), calcola S(i) = X(i) + Y(i) e memorizza il risultato nella propria memoria.
* **Implementazione**:

  * Somma dei valori realizzata con approccio comportamentale.
  * Entrambi i nodi includono un contatore per scandire la trasmissione/ricezione e terminare la comunicazione.

---

**Nota**: Tutti i moduli e i testbench si trovano nelle rispettive cartelle; questo README fornisce una panoramica generale dell’esercizio.
