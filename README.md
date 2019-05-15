# SVentola
Variatore di giri per ventole (motori CC)

"Il mio amico Silvio, ogni volta che gli chiedo una cosa cerca di farla e cerca di farla al meglio."

Lo scopo:
Variare i giri di una ventola che può essere a due o a tre fili.


Premessa

- Della ventola sappiamo poco e niente ovvero, non sappiamo la corrente di lavoro e per la tensione sappiamo solo che può andare da 5 a 15V.
- Non è importante sapere a quanti giri gira la ventola ma, se è possibile, è utile sapere se gira (gestione del terzo filo).
- Il controllo deve avvenire tramite un attuatore rotativo che possibilmente deve essere a giro continuo così da ridurre la possibilità di danneggiamenti involontari durante l'uso
- Il dispositivo deve:
  - costare poco,
  - essere realizzato con materiale reperibile facilmente,
  - essere riproducibile facilmente,
  - non essere ingombrante ne eccessivamente energivoro.

Scelte

Dopo aver dimensionato e realizzato un paio di circuiti basati su componenti discreti (regolatori di tensione e pompe di corrente), si è giunti alla conclusione che, seppur si riuscisse a realizzare una soluzione economica, compatta e funzionale, la riproduzione avrebbe richiesto un livello di competenze, tempo e abilità non sempre disponibili e, anche in caso di cattivo funzionamento, la diagnostica avrwebbe richiesto un livello di conoscenza e un minimo di strumentazione non sempre presenti. Ne è derivata la scelta di prendere in considerazione un dispositivo basato su un controllore e un driver per motori scegliendo il materiale fra quelli diffusamente offerti dal mercato per l'automazione e/o la robotica.

Anche quando abbiamo valutato le periferiche (attuatore rotativo e spia di funzionamento) i fattori funzionalità/reperibilità hanno abbundantemente giustificato la scelta di andare verso dispositivi ad alto contenuto tecnologico piuttosto che indirizzarsi verso elementi discreti come potenziometri e LED.

Dopo una lunga analisi delle caratteristiche tecniche, dimensionali e commerciali dei (molti) componenti offerti dal mercato la scelta è andata verso i seguenti elementi:
- Unità centarle WeMos D1 mini basato su processore ESP8266,
- Unità di potenza WeMos D1 mini motor controller,
- Attuatore encoder rotativo precablato
- display strip da 8 Neopixel Adafruit o equivalente
