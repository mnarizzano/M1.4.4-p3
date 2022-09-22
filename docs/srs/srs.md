![alt tag](https://github.com/mnarizzano/M1.4.4-p3/blob/main/docs/srs/imgs/usecases.png)


## 2 	Scenari 
## 2.1 Studente

1. Caso di studente: Iscrizione a corso
				
		scenario principale:
		1.1)- lo studente chiede di essere iscritto ad un corso	
		1.1.2)- l'amministrazione chiede i documenti e verifica i requisiti dello studente
		1.3)- L'amministrazione iscrive lo studente al corso
		1.4)- il sistema registra lo studene iscritto
		1.5)- studente iscritto

		Scenario alternativo			
		1.3b)- requisiti non idonei
		1.4b)- studente non iscritto
		Post condizione-
		Viene creato un profilo studente, con tutte le informazioni personali e gli vengono assegnate
		delle credenziali di accesso.
		
2. Caso di studente: Cancellazione da corso

		scenario principale:
		2.1)- lo studente chiede di essere cancellato da un corso
		2.2)- l'amministrazione cancella studente dal corso
		2.3)- il sistema cancella lo studente 
		2.4)- l'utente cancellato
	
3. Caso di studente: Visualizzazione corsi

		scenario principale
		3.1)- lo studente chiede di visualizzare i corsi a cui è iscritto
		3.2)- il sistema verifica che lo studente esista
		3.3)- Utente esiste
		3.4)- il sistema fa visualizzare i corsi 
		3.5)- l'utente visualizza i corsi
	
		scenario alternativo
		3.3b)- utente non esiste
		3.4b)-  l'utente non visualizza i corsi

4. Caso di studente: lista esami superati

		scenario principale		
		4.1)- lo studente chiede lista degli esami superati
		4.2)- il sistema chiede nome utente e password
		4.3)- loggin riuscito
		4.4)- il sistema va visualizzare esami superati
		4.5)- studente visualizza esami superati

		scenario alternativo:		
		4.3b)- loggin non riuscito
		4.4b)-  password sbagliata
		4.5b)- studente non visualizza esami superati
		Post condizione-
		Viene stampato documento con esami superati

		scenario alternativo 2:
		4.3c)- loggin non riuscito
		4.4c)- nome utente non trovato
		4.5c)- studente non visualizza esami superati 

5. Caso di studente: lista esami

		5.1) lo studente chiede di visualizzare lista esami dispnibili
		5.2) lo studente insesciri le credenziali di autenticazione
		5.3) loggin riuscito
		5.4) lo studente visualizza gli esami disponibili.
		5.5) lo studente prenota un esame
		5.6) il sistema registra lo studente all'esame
		5.7) studente registrato
		Post condizione-
		viene stampata la data dell'esame.

## 2.2 - Docente

1. Caso docente: Visualizzazione dei corsi di cui è docente:

		Scenario principale:
		1.1)-Il sito richiede al docente utente e password
		1.2)-Il docente inserisce utente e password correttamente
		1.3)-Il docente entra nel sito
		1.4)-Il docente riesce a visualizzare correttamente i corsi di cui è insegnante
		
		Caso alternativo:
		1.2b)- Il docente inserisce utente e/o password sbagliate
		1.3b)-  Il docente non riesce ad entrare con i dati correnti 
		1.4b)-  Il docente reimposta la password
		1.5b)-  Il docente riesce ad entrare nel sito
	
2. Caso docente: indire esame per corso

		Scenario principale:
		2.1)- Il docente seleziona il corso di cui vuole indire l’esame
		2.2)- Il docente chiede date e orari all’amministrazione
		2.3)- L’amministrazione conferma date e orari al docente
		2.4)- Il docente crea l’esame
		
		Scenario alternativo:
		2.3b) L’amministrazione non conferma le date e orari al docente
		2.b)-  Il docente chiede le date e orari disponibili all’amministrazione
		2.5b)-  L’amministrazione consegna il modulo con le date e orari disponibili al docente
		2.6b)-  Il docente sceglie le date e orari opportuni e le consegna all’amministrazione
		2.7b)- L’amministrazione conferma le date e orari
		2.8b)- Il docente crea l’esame
	
3. Caso docente: Assegnazione voti

		Scenario principale
		Pre condizione = Il docente ha già corretto gli esami
		3.1)- Il docente seleziona l’esame del corso di cui vuole mettere i voti
		3.2)- Il docente seleziona l’appello di quel relativo esame
		3.3)- Il docente selezione lo studente a cui deve mettere il voto
		3.4)- il docente mette il voto

4. Caso docente: Studenti iscritti ad un esame 

		Scenario principale
		Pre condizione = lo studente deve essere iscritto all’esame
		4.1)- Il docente seleziona l’esame di cui vuole la lista degli iscritti
		4.2)- Il docente seleziona l’appello
		4.3)- Al docente viene visualizzata la lista degli 
		
		
## 2.3 - Amministrazione  

1. caso di Amministrazione: creazione studente

		- scenario principale  (1a):  
		1.1)   studente richiede di iscriversi
		1.2)   amministrazione richiede documenti per valutarne requisiti 
		1.3a)  requisiti studente idonei 
		1.4a)  amministrazione registra studente all' ateneo

		- scenario alternativo (1b): 
		1.3b)  requisiti studente NON idonei
		1.4b)  amministrazione informa che studente non ha i requisiti necessari
 
2. caso di Amministrazione: cancellazione studente

		-scenario principale:   
		2.1)   studente richiede di cancellarsi dal corso
		2.2)   amministrazione avvia le pratiche per la cancellazione dello studente dai registri

3. caso di Amministrazione: creazione corso:
			
		- scenario principale  (3a):  
		3.1)   Amministrazione riceve richieste da parte del ministero
		3.2)   Amministrazione valuta che siano presenti sia il personale che le risorse necessarie
		3.3a)  amministrazione valuta positivamente
		3.4a)  amministrazione istituisce il corso 

		- scenario alternativo (3b):
		3.3b)  amministrazione valuta negativamente
		3.4b)  amministrazione informa ministero della mancanza di risorse


4. caso di Amministrazione: modifica corso:

		- scenario principale  (4a): 
		4.1)   valutazione delle motivazioni che ne causerebbero la modifica
		4.2a)  amministrazione valuta positivamente le motivazioni 
		4.3a)  amministrazione informa studenti e docenti dei cambiamenti
		4.4a)  amministrazione procede effettivamente all' applicazione delle modifiche
			
		-scenario secondario: (4b):  
		4.2b)  amministrazione non ritiene valide le motivazioni 
		4.3b)  amministrazione informa ministero dell' impossibilità di procedere alla modifica

5. caso di amministrazione: cancellazione corso:

		-scenario principale   
		5.1)   amministrazione Valuta le motivazioni se non richiesto dal ministero
		5.2)   amministrazione informa preventivamente studenti e docenti 
		5.3)   amministrazione procede effettivamente alla cancellazione

6. caso di Amministrazione: creazione docente:
	
		- scenario principale  (6a): 
		6.1)   amministrazione valuta la candidatura 
		6.2a)  amministrazione assume il docente che possiede i requisiti necessari

		- scenario secondario  (6b):
		6.2b)  amministrazione non assume il docente che difetta dei requisiti necessari

7. caso di amministrazione: cancellazione docente:

		- scenario principale  (7a):
		7.1)   amministrazione valuta le motivazioni per procedere alla cancellazione
		7.2)   amministrazione valuta necessario sostituire vecchio docente
		7.3a)  amministrazione si accorda con nuovo docente
		7.4a)  amministrazione licenzia vecchio docente

		- scenario secondario  (7b):			
		7.3b)  amministrazione valuta non necessario sostituire vecchio docente
		7.4b)  amministrazione licenzia vecchio docente






	

