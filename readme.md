

Milestone 1
Replica della grafica con la possibilità di avere messaggi scritti dall’utente (verdi) e dall’interlocutore (bianco) assegnando due classi CSS diverse
Visualizzazione dinamica della lista contatti: tramite la direttiva v-for, visualizzare nome e immagine di ogni contatto


Milestone 2
Visualizzazione dinamica dei messaggi: tramite la direttiva v-for, visualizzare tutti i messaggi relativi al contatto attivo all’interno del pannello della conversazione
Click sul contatto mostra la conversazione del contatto cliccato




Milestone 3
Aggiunta di un messaggio: l’utente scrive un testo nella parte bassa e digitando “enter” il testo viene aggiunto al thread sopra, come messaggio verde
Risposta dall’interlocutore: ad ogni inserimento di un messaggio, l’utente riceverà un “ok” come risposta, che apparirà dopo 1 secondo.


Milestone 4
Ricerca utenti: scrivendo qualcosa nell’input a sinistra, vengono visualizzati solo i contatti il cui nome contiene le lettere inserite (es, Marco, Matteo Martina -> Scrivo “mar” rimangono solo Marco e Martina)


Milestone 5 - opzionale
Cancella messaggio: cliccando sul messaggio appare un menu a tendina che permette di cancellare il messaggio selezionato

Visualizzazione ora e ultimo messaggio inviato/ricevuto nella lista dei contatti
--------------------------------
esecuzione milestone 1:
-pensare alla struttura nella sezione contatti(scrivere su foglio)
-problemi da risolvere:
(stampare ultimo msg nel div contact)
aggiungere bottone invia nell'input-chat
-capire come strutturare messaggi in chat
------------------------------
milestone 2:
devo fare in modo di visualizzare i messaggi relativi al  contatto cliccato.
Per ora ho messo come segnaposto la chat del primo contatto ma devo creare una funzione che al click dell'utente nei contatti vada a mostrare la relativa chat.
cose che serviranno :
 
-scrivere funzione nei methods che vada ad alterare la chat mostrando i messaggi relativi a quell'utente  

-funzione @click sui div .contact

che scrivo nella funzione?

f_chat:nome funzione
cosa vado ad alterare inanzitutto?
-vado ad alterare nella parte a destra:
-l'immagine con nome ed i messaggi in chat

come le riconosco le varie chat?
dall'indice della persona nel contacts: se è Michelel'indice è 0 e così via 

potrei aggiungere negli oggetti persona un booleano di nome visualizzato che cambia al click?
o aggiungo un'indice utenteselezionato in ogni persona con un valore e in base all'utente selezionato vado a cliccare ?

potrei andare a cambiare l'indice (mettendo l'indice come argomento funzione)
