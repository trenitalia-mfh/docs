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
Il progetto TrenoFacile si propone come un insieme di funzionalità da integrare nell’attuale applicazione mobile Trenitalia.

In particolare:

Per i passeggeri
- Un arricchimento dell'applicazione Trenitalia con nuove funzionalità
- Un chatbot Facebook Messenger

Il cui scopo è rendere più piacevole e completa l’esperienza di viaggio con Trenitalia.


Per lo staff Trenitalia
- Un’applicazione dedicata ai controllori a bordo treno

Il cui scopo è snellire e rendere efficaci le procedure di controllo a bordo treno.


## Applicazione Trenitalia (per i passeggeri)
La nuova applicazione, oltre a fornire le funzionalità già presenti, è pensata per:
- Realizzare check-in automatico a bordo treno
- Offrire interazione vocale con il nuovo sistema TrenoFacile (conoscere stato del treno, ottenere offerte di prodotti ancillari al viaggio)
- Richiedere l'intervento di un controllore a bordo treno per un problema con il viaggio

### Check-in automatico
L’applicazione, installata sullo smartphone del passeggero che ha acquistato un biglietto, invierà la posizione del passeggero il giorno del viaggio e all’approssimarsi dell’orario di partenza. Il monitoring continuerà fino a tot minuti dalla partenza del treno per assicurarsi che il passeggero sia effettivamente su di esso. Dopo di che verrà inviata, in automatico e senza azioni da parte del passeggero, la richiesta di check-in al server per confermare che il passeggero si trovi a bordo. Ad operazione completata l’utente riceverà una notifica di benvenuto a bordo che lo inviterà ad aprire la dashboard di viaggio.

Vantaggi del check-in automatico:
- Minore interazione utente-controllore
- Miglioramento delle statistiche di traffico per i treni regionali
- Invalidazione dei biglietti su treni regionali

### Reminder di check-in
Se l’applicazione è installata sullo smartphone del passeggero ma NON è stata data la possibilità di accedere alla posizione del GPS, l’applicazione, tenendo conto della lista di biglietti acquistati, invierà una notifica push entro pochi minuti dall’orario di partenza del treno, per ricordare al passeggero che può effettuare il check-in in maniera autonoma per quel singolo viaggio.

### Dashboard di viaggio
Per i passeggeri che avranno completato il check-in, l’applicazione potrà fornire informazioni relative al treno e proporre prodotti ancillari, sia a bordo treno che post-viaggio (es. menù del bistrot o del ristorante a bordo, offerta di hotel, taxi o servizi nella città di destinazione, elenco di eventi interessanti nella città di destinazione nel periodo di viaggio).
I suggerimenti riguardo i prodotti ancillari saranno profilate rispetto a parametri quali le preferenze dell’utente, lo storico viaggi, dati ricavati dai social network, etc.

### A portata di voce
Sfruttando le API speech2text offerte dagli smartphone di recente generazione (Siri, Google Now ecc) sarà possibile richiedere a bordo treno informazioni su viaggio, dopo aver effettuato il check-in.

Ad esempio sarà possibile fare domande quali ‘A che velocità stiamo andando?’, ‘Che cosa mi offre il bar di bordo?’ oppure ‘Prenota un taxi a Milano per l’orario di arrivo’ semplicemente interagendo con il proprio smartphone.

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
