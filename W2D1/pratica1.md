Protocolli del livello Dati
===

sottolivello MAC
---

Nel layer 2 del modello ISO/OSI, il *Medium Access Control* controlla l'accesso al mezzo trasmissivo da parte dei dispositivi della rete locale.
Ogni dispositivo viene identificato da un MAC address univoco a 48 bit, rappresentato solitamente in esadecimale con la seguente forma

    aa:bb:cc:dd:ee:ff

I primi 24 bit sono assegnati da IEEE ai produttori di schede di rete, mentre gli ultimi 24 vengono scelti dal produttore.

Possibili attacchi: MAC spoofing (che può anche essere non malevolo, per esempio il MAC address è generato casualmente negli ultimi android)

Esempi di protocolli che adibiscono alla funzione MAC:

- CSMA/CA carrier sense multiple access with collision avoidance: utilizzato soprattutto in reti senza fili, come nello standard IEEE 802.11 (Wi-Fi), in cui i nodi controllano che il mezzo trasmissivo sia disponibile prima di spedire dati
- CSMA/CD carrier sense multiple access with collision detection: usato una volta su reti ethernet, quando ancora si usavano gli hub. Da quando ci sono gli switch che comunicano full-duplex (ricezione e trasmissione contemporanea), è caduto in disuso in quanto non più necessario.


ARP: Address Resolution Protocol
---

Questo protocolllo di servizio permette di scoprire il MAC associato a un indirizzo IP.  Su linux è possibile usare il comando `arping` da riga di comando.


Altri protocolli
---

- Ethernet, IEEE 802.3; protocollo ampliamente usato per le reti locali (LAN)
- Token ring, IEEE 802.5; 
