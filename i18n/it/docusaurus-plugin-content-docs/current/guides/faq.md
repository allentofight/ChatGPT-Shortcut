# Domande frequenti

## Perché le parole suggerite sono in inglese?

AiShort è stato creato per facilitare l'uso di ChatGPT da parte di persone non native di lingua inglese. Tuttavia, tutte le parole suggerite sono in inglese. Ciò è dovuto al fatto che ChatGPT ha una migliore comprensione dell'inglese rispetto alle altre lingue. Anche MOSS, il primo modello di linguaggio cinese per il dialogo su larga scala, riconosce che le sue risposte in inglese sono superiori a quelle in cinese. Pertanto, si consiglia di utilizzare parole suggerite in inglese. (MOSS non è più disponibile)

Sebbene l'uso di parole suggerite in altre lingue possa dare risultati decenti, i risultati possono variare significativamente quando si inseriscono le stesse sollecitazioni non in inglese. Poiché la comprensione di ChatGPT delle sollecitazioni non in inglese varia ogni volta, si consiglia di utilizzare sollecitazioni in inglese per sollecitazioni orientate alla produttività al fine di ottenere l'output desiderato. Inoltre, le risposte generate da sollecitazioni in inglese saranno probabilmente in inglese. È possibile specificare la lingua di risposta come cinese aggiungendo "rispondi in cinese" alla fine della sollecitazione. Se la tua lingua madre è diversa, sostituisci "cinese" con la tua lingua madre.

## Devo inserire la sollecitazione ogni volta?

Nell'API, puoi impostare la sollecitazione come "sollecitazione di sistema", in modo da non dover inserire la sollecitazione ogni volta. ChatGPT seguirà le istruzioni basate sulla sollecitazione di sistema.

Nella versione web di ChatGPT, se non hai cambiato la sollecitazione principale, puoi semplicemente racchiudere il contenuto della risposta successiva tra virgolette, eliminando la necessità di inserire la sollecitazione ogni volta. Quando la risposta generata non corrisponde ai requisiti della sollecitazione, significa che ChatGPT ha dimenticato la sollecitazione e, in tali casi, è necessario reinserire la sollecitazione per riorientarlo. Inoltre, ogni link di conversazione è unico e puoi salvare le conversazioni frequentemente utilizzate come segnalibri per un uso futuro.

## Ritardo nella ricerca del metodo di input

La funzione di ricerca si basa sulla vetrina di Docusaurus e presenta un problema con la perdita di focus del metodo di input sul lato del PC. Dopo aver segnalato il problema a Docusaurus, hanno menzionato di voler cercare di risolverlo, ma finora il problema rimane irrisolto, con il commento: "FWIW, dovresti comunque non utilizzare il cinese, poiché la vetrina non è localizzata." Pertanto, ho categorizzato il componente di ricerca in due tipi: mobile e PC. La logica di ricerca per i dispositivi mobili rimane invariata, mentre per la navigazione su PC con una larghezza dello schermo superiore a 768px, ho introdotto la funzione "debounce" per affrontare il problema del metodo di input. Tuttavia, questo introduce due problemi sul lato del PC: l'input non in inglese deve essere completato entro 800 millisecondi e l'aggiornamento della ricerca su PC cambia da istantaneo a un ritardo di 800 millisecondi. Se hai una soluzione migliore, fornisci un feedback.

## Emissione di informazioni false

Anche se ChatGPT è molto potente, non è infallibile. A volte può emettere informazioni false. Ad esempio, quando ho avuto bisogno di inserire centinaia di informazioni in AiShort, ho fatto convertire i dati da ChatGPT in un formato specifico. Tuttavia, durante il processo di conversione, ho notato che ChatGPT aveva scritto in modo inaccurato alcune delle informazioni. Ad esempio, una dicitura nel testo era "critico cinematografico", ma ChatGPT l'ha cambiata in "critico del cinema". Sebbene ciò potrebbe non avere alcun impatto sul testo stesso, potrebbe causare un errore quando viene utilizzato nel codice. Pertanto, quando si utilizza ChatGPT, è essenziale rivedere il suo output.

## Le parole suggerite non funzionano bene

Tutte le parole suggerite sono tratte da Internet e vengono aggiornate regolarmente. Sebbene abbia testato ogni parola suggerita, le prestazioni effettive possono deviare a seconda delle esigenze specifiche. Se scopri errori, hai idee creative o possiedi buone parole suggerite, non esitare a fornire feedback e contribuire sulla [pagina di GitHub](https://github.com/allentofight/ChatGPT-Shortcut/discussions/11).

Se stai riassumendo o condensando informazioni, puoi utilizzare GPT per raffinare ulteriormente le risposte originali, migliorando così l'accuratezza delle risposte. Inoltre, le parole suggerite non servono solo a scopi produttivi, ma aiutano anche ad ampliare il pensiero, stimolare la creatività, considerare i problemi da diverse prospettive e risolvere questioni che sono facilmente trascurate durante il processo di pensiero.
