# boolzapp ITA

questo progetto prevede la replica layout di Whatsapp utilizzando come framework Vuejs.
come funzionalità abbiamo la ricerca nei contatti sulla parte sinistra mentre sulla parte destra abbiamo la schermata della chat nella quale possiamo inviare un messaggio che ci risponderà in automatico ok .
Questa repo fa parte dei lavori effettuati durante il corso di web development organizzato da Boolean. con questa repo nello specifico ho capito quali possono essere le funzionalità di Vue e di come questo framework sia un grande strumento nella realizzazione di siti web e di web app.
La difficoltà riscontrata in questo esercizio è stata l'applicazione delle logiche di Vue in un contesto "vero", quindi capire come implementare la ricerca dei contatti e capire come strutturare l'input dei messaggi. 



# boolzapp ENG
This project involves replicating the Whatsapp layout using Vuejs as the framework. The features include searching contacts on the left side, while on the right side, we have the chat screen where we can send a message that will automatically reply 'ok'. This repository is part of the work done during the web development course organized by Boolean. With this specific repository, I understood the potential functionalities of Vue and how this framework is a great tool in building websites and web apps. The challenge faced in this exercise was applying Vue logics in a "real" context, understanding how to implement contact search and structuring message inputs.


# milestone ed esecuzione  
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
dall'indice della persona nel contacts: se è Michele l'indice è 0 e così via 

potrei aggiungere negli oggetti persona un booleano di nome visualizzato che cambia al click?
o aggiungo un'indice utenteselezionato in ogni persona con un valore e in base all'utente selezionato vado a cliccare ?

potrei andare a cambiare l'indice (mettendo l'indice come argomento funzione)
--------------------------

esecuzione milestone 3:
devo aggiungere un messaggio in pagina da parte dell'utente 
cosa ho bisogno:
-input(ce l'ho)
-variabile da collegare all'utente(manca)
-funzione (da creare)
-collegare funzione al'input tramite @keyenter(volendo mettere anche all'icona messaggio@click
)

-nella funzione temporale :
-creo un data usermsg con valori simili a inputmsg(cambiare status da sent a received)
------------------
milestone 4
devo visualizzare solo i contatti che iniziano con il testo scritto nell'input
cosa mi serve:
-input nella parte contatti(c'é)
-data per salvare quello che c'è scritto nell'input
-confrontare quel dato con startwith il quale restituirà booleano
-porre condizione

come devo ragionare?
scrivendo nell'input, devo confrontare la stringa scritta nell'input con il nome dei contatti 
come faccio questo confronto?