# Trenitalia Moving Forward Hackaton 2017

## Scopo del progetto

Creare un sistema per il miglioramento dell’esperienza del passeggero prima, durante e dopo il viaggio tramite l’utilizzo di sistemi automatici, offrendo funzionalità quali:
- Check-in automatico del biglietto senza il bisogno di interazioni da parte del passeggero
- Interazione automatizzata (vocale e testuale) ad eventuali richieste del passeggero
- Risoluzione di problemi di viaggio evitando l’intervento di un controllore od un assistente di viaggio (info sulle commodities, sul viaggio)
- Promozione di prodotti ancillari al viaggio


## Definizione attori

### Passeggero

Colui che acquista il titolo di viaggio ed utilizza i sistemi di trasporto Trenitalia

### Controllore

Membro dello staff Trenitalia che si occupa di verificare l’occupazione dei posti su un treno in viaggio


## Soluzione proposta

Viene proposta e dettagliata una soluzione che integri:

Per i passeggeri
- Una ‘nuova’ applicazione Trenitalia
- Un chatbot Facebook Messenger

Il cui scopo è rendere più piacevole e completa l’esperienza di viaggio con Trenitalia.


Per lo staff Trenitalia
- Un’applicazione dedicata ai controllori a bordo treno

Il cui scopo è snellire e rendere efficaci le procedure di controllo a bordo treno.


## Nuova applicazione Trenitalia (per i passeggeri)

La nuova applicazione, oltre a fornire le funzionalità già presenti, è pensata per:
- Realizzare check-in automatico a bordo treno
- Offrire interazione vocale con il nuovo sistema TrenoFacile (conoscere stato del treno, ottenere offerte di prodotti ancillari al viaggio)
- Richiedere l'intervento di un controllore a bordo treno per un problema con il viaggio

### Check-in automatico
L’applicazione, installata sullo smartphone del passeggero che ha acquistato un biglietto, invierà la posizione del passeggero il giorno del viaggio e all’approssimarsi dell’orario di partenza. Il monitoring continuerà fino a tot minuti dalla partenza del treno per assicurarsi che il passeggero sia effettivamente sul treno, dopo di che verrà inviata (in automatico e senza azioni da parte del passeggero) la richiesta di check-in al server per confermare che il passeggero si trovi a bordo.

### Reminder di check-in
Se l’applicazione è installata sullo smartphone del passeggero ma NON è stata data la possibilità di accedere alla posizione del GPS, l’applicazione, tenendo conto della lista di biglietti acquistati, invierà una notifica push entro pochi minuti dall’orario di partenza del treno, per ricordare al passeggero che può effettuare il check-in in maniera autonoma per quel singolo viaggio.

### Promozione di prodotti ancillari
Per i passeggeri che avranno completato il check-in, l’applicazione potrà fornire informazioni relative a prodotti ancillari al viaggio, sia a bordo treno che post-viaggio (es. menù del bistrot o del ristorante a bordo, offerta di hotel, taxi o servizi nella città di destinazione, elenco di eventi interessanti nella città di destinazione nel periodo di viaggio).

### Interazione vocale
Sfruttando le API speech2text offerte dagli smartphone di recente generazione, il passeggero potrà interagire con l’applicazione anche mediante voce, per azioni quali:
- Recupero dell’elenco di biglietti
- Recupero dello stato di un treno
- Check-in volontario a bordo treno

## Chatbot Facebook Messenger (per i passeggeri)
Per coloro i quali non abbiano a disposizione uno smartphone compatibile con l’applicazione o non vogliano installarla, viene offerto un chatbot su Facebook Messenger in grado di fornire, mediante messaggi di testo, le stesse funzionalità ottenute tramite l’interazione vocale della nuova applicazione.

Il chatbot, inoltre, avendo un canale diretto con il passeggero, potrà comportarsi come l’applicazione ed inviare, una volta effettuato il check-in, messaggi contenenti le offerte dei prodotti ancillari al viaggio.

## Applicazione di Controllo (per lo staff a bordo)
Presumendo che i controllori abbiano a disposizione un device mobile (smartphone o tablet), l’applicazione di controllo mostra lo stato dei posti per ogni carrozza di un determinato treno.

Per ogni carrozza vengono mostrati tutti i posti, marcati come
- Liberi: non venduti
- Check-in effettuato: posti venduti e per i quali non è necessario effettuare controllo
- Da controllare: posti venduti per i quali è necessario effettuare controllo manuale

L’applicazione permetterà al controllore che la sta utilizzando di variare lo stato dei posti a seconda della necessità (es. da ‘da controllare’ a ‘controllati’, una volta fatto il controllo manuale del biglietto del passeggero).
