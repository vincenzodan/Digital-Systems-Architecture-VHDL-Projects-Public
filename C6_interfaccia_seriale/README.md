# Interfaccia Seriale – UART-RS232

Questo capitolo raccoglie gli esercizi sull’**interfaccia seriale**, sviluppati in **VHDL** e testati mediante simulazione.

## Esercizio 10 – Comunicazione tra due unità seriali

* **Obiettivo**: Progettare e simulare un sistema composto da due unità, A e B, che comunicano tra loro mediante interfaccia seriale UART-RS232.
* **Architettura**:

  * **Unità A**: contiene una ROM di 8 locazioni da 1 byte ciascuna, un contatore `CONT_A` per scandire le locazioni della ROM e un componente `UART_A`.
  * **Unità B**: contiene una memoria `MEM` di 8 locazioni da 1 byte ciascuna, un contatore `CONT_B` per scandire le locazioni della MEM e un componente `UART_B`.
* **Funzionamento**:

  * Entrambe le unità condividono lo stesso clock.
  * Quando il segnale `WR` viene asserito in A, un byte della ROM viene inviato a B.
  * L’unità B riceve il byte e lo salva nella memoria interna `MEM`.
* **Implementazione**: Utilizzo della componente fornita `RS232RefComp.vhd` come base per la UART, con aggiunta di contatori e logica di controllo per la trasmissione e ricezione dei dati.

---

**Nota**: Tutti i moduli, testbench e memorie si trovano nelle rispettive cartelle; questo README fornisce una panoramica generale dell’esercizio.
