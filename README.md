# EasyPick
Le informazioni contenute nel presente manuale sono soggette a modifiche senza preavviso e non devono essere considerate vincolanti per ABB Italia S.p.A. ABB Italia S.p.A. non si assume alcuna responsabilità per eventuali errori nel presente manuale.

Salvo quanto espressamente indicato nel presente manuale, ABB Italia S.p.A. non concede alcuna altra garanzia in relazione al prodotto in merito a eventuali perdite, danni a persone o beni, idoneità per uno scopo specifico o altro. In nessun caso ABB Italia S.p.A. potrà essere ritenuta responsabile per eventuali danni accidentali o consequenziali dovuti all'utilizzo del presente manuale e dei prodotti in esso descritti.

Né questo manuale, né alcuna sua parte possono essere riprodotti o ricopiati senza il consenso scritto da parte di ABB Italia S.p.A. Delle copie supplementari di questo manuale possono essere ottenute da ABB Italia S.p.A.

© ABB Italia 2023
ABB Italia S.p.A. – Robotics Division 
Via Luciano Lama 33
20099 Sesto San Giovanni (MI) 
Italy

# Descrizione
EasyPick (EP) è un'opzione RobotWare (RW) per le versioni 6 e 7. L'obiettivo è la gestione automatica della coda di uno o più conveyor, senza lo sviluppo di alcun codice RAPID specifico o la 
necessità di hardware aggiuntivo.
Essa funziona sia per conveyor lineari e circolari, ed è totalmente integrata nel controllore del robot.


# Limitazioni

| Parametro             | Limiti                                                                                                  |
|------------------------|--------------------------------------------------------------------------------------------------------|
| **Numero di robot** | 2|
| **Numero di conveyor**|3|
| **Numero di camere** | 3 |
| **Numero di oggetti per conveyor** | 300|
| **Numero di oggetti per immagine** | 30 |
| **Numero di oggetti saltati (skip)** | 100 |
| **Tempo di elaborazione** | **Inferiore alla distanza di trigger** |
|**Index Conveyor non supportato** |  |
|**Telecamere Client TP/IP non supportato**|  |


# Requisiti
| Opzione      | RW6 | RW7   |
|-------------|----|--------|
|**RW Add-In Prepared**| 988-1 |3121-1|
|**Tracking Unit (DSQC2000)** |1551-1 |3042-1|
|**Tracking Unit Interface** |1552-1* |/|
|**Conveyor Tracking** |606-1 |3103-1|
|**Multitasking** |623-1 |3114-1|
|**Ethernet Extension Switch (1 IRB)** |/ |3014-1**|

**Ethernet Switch (2 IRB)** Device Hardware QOS (Quality of Service) switch is recommended.

(*) Solo se non è presente l’opzione 1551-1.
(**) Solo nel caso in cui la DSQC2000 dovrà essere collegata alla Private Network.


Se viene utilizzata la Visione Integrata, sono necessarie le seguenti opzioni:
| Opzione      | RW6 | RW7   |
|-------------|----|--------|
|**Integrated vision** |988-1| 3127-1|


Se viene utilizzata la Visione Esterna, sono disponibili le seguenti opzioni:

| Opzione      | RW6 | RW7   |
|-------------|----|--------|
|**Profinet Controller/Device** |888-2 |3020-1|
|**Profinet Device** |888-3 |3020-2|
|**Profinet Anybus Device**| 840-3| /|
|**Ethernet/IP Anybus Adapter**| 840-1| 3024-1|
|**Ethernet/IP Scanner/Adapter**| 841-1 |3024-2|
|**TCP/IP**| 616-1| /|

