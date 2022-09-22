![alt tag](https://github.com/mnarizzano/M1.4.4-p3/blob/main/docs/srs/imgs/usecases.png)


## 2 	Scenari 
## 2.1 Studente

		Caso di studente: Iscrizione a corso
		scenario principale:
		1)- lo studente chiede di essere iscritto ad un corso	
		2)- l'amministrazione chiede i documenti e verifica i requisiti dello studente
		3)- L'amministrazione iscrive lo studente al corso
		4)- il sistema registra lo studene iscritto
		5)- studente iscritto

		Scenario alternativo			
		3b)- requisiti non idonei
		1)- studente non iscritto
		Post condizione-
		Viene creato un profilo studente, con tutte le informazioni personali e gli vengono assegnate
		delle credenziali di accesso.

		Caso di studente: Cancellazione da corso
		scenario principale:
		1)- lo studente chiede di essere cancellato da un corso
		2)- l'amministrazione cancella studente dal corso
		3)- il sistema cancella lo studente 
		4)- l'utente cancellato
	
		caso di studente: Visualizzazione corsi
		scenario principale
		1)- lo studente chiede di visualizzare i corsi a cui è iscritto
		2)- il sistema verifica che lo studente esista
		3)- Utente esiste
		4)- il sistema fa visualizzare i corsi 
		5)- l'utente visualizza i corsi
	
		scenario alternativo
		3b)- utente non esiste
		1)-  l'utente non visualizza i corsi

		Caso di studente: lista esami superati
		scenario principale		
		1)- lo studente chiede lista degli esami superati
		2)- il sistema chiede nome utente e password
		3)- loggin riuscito
		4)- il sistema va visualizzare esami superati
		5)- studente visualizza esami superati

		scenario alternativo:		
		3b)- loggin non riuscito
		1)-  password sbagliata
		2)- studente non visualizza esami superati
		Post condizione-
		Viene stampato documento con esami superati

		scenario alternatio 2:
		3c)- loggin non riuscito
		1)- nome utente non trovato
		2)- studente non visualizza esami superati 

		Caso di studente: lista esami
		1) lo studente chiede di visualizzare lista esami dispnibili
		2) lo studente insesciri le credenziali di autenticazione
		3) loggin riuscito
		4) lo studente visualizza gli esami disponibili.
		5) lo studente prenota un esame
		6) il sistema registra lo studente all'esame
		7) studente registrato
		Post condizione-
		viene stampata la data dell'esame.

## 		Scenari 2.2 Docente

		Caso docente: Visualizzazione dei corsi di cui è docente:
		Scendario principale:
		
		1)-Il sito richiede al docente utente e password
		2)-Il docente inserisce utente e password correttamente
		3)-Il docente entra nel sito
		4)-Il docente riesce a visualizzare correttamente i corsi di cui è insegnante
		
		Caso alternativo:
		2a)- Il docente inserisce utente e/o password sbagliate
		3)-  Il docente non riesce ad entrare con i dati correnti 
		4)-  Il docente reimposta la password
		5)-  Il docente riesce ad entrare nel sito
	
		caso docente: indire esame per corso
		scenario Principale:
		1)- Il docente seleziona il corso di cui vuole indire l’esame
		2)- Il docente chiede date e orari all’amministrazione
		3)- L’amministrazione conferma date e orari al docente
		4)- Il docente crea l’esame
		
		Caso alternativo:
		3a) L’amministrazione non conferma le date e orari al docente
		4)-  Il docente chiede le date e orari disponibili all’amministrazione
		5)-  L’amministrazione consegna il modulo con le date e orari disponibili al docente
		6)-  Il docente sceglie le date e orari opportuni e le consegna all’amministrazione
		7)- L’amministrazione conferma le date e orari
		8)- Il docente crea l’esame
	
		Caso docente: Assegnazione voti
		Pre condizione = Il docente ha già corretto gli esami
		1)- Il docente seleziona l’esame del corso di cui vuole mettere i voti
		2)- Il docente seleziona l’appello di quel relativo esame
		3)- Il docente selezione lo studente a cui deve mettere il voto
		4)- il docente mette il voto

		CAso docente: Studenti iscritti ad un esame 
		Pre condizione = lo studente deve essere iscritto all’esame
		1)- Il docente seleziona l’esame di cui vuole la lista degli iscritti
		2)- Il docente seleziona l’appello
		3)- Al docente viene visualizzata la lista degli 
		
		
## Amministrazione 2.3 

1. caso di Amministrazione, creazione studente
		        - scenario principale  (1a):  
						1.1)   studente richiede di iscriversi
				 	        1.2)   amministrazione richiede documenti per valutarne requisiti 
					        1.3a)  requisiti studente idonei 
					        1.4a)  amministrazione registra studente all' ateneo

			- scenario alternativo (1b): 
					        1.3b)  requisiti studente NON idonei
						1.4b)  amministrazione informa che studente non ha i requisiti necessari
 
2. caso di Amministrazione, cancellazione studente:

			-scenario principale:   
						2.1)   studente richiede di cancellarsi dal corso
						2.2)   amministrazione avvia le pratiche per la cancellazione dello studente dai registri

3. caso di Amministrazione, creazione corso:
			
			- scenario principale  (3a):  
						3.1)   Amministrazione riceve richieste da parte del ministero
						3.2)   Amministrazione valuta che siano presenti sia il personale che le risorse necessarie
						3.3a)  amministrazione valuta positivamente
						3.4a)  amministrazione istituisce il corso 

			- scenario alternativo (3b):
						3.3b)  amministrazione valuta negativamente
						3.4b)  amministrazione informa ministero della mancanza di risorse


4. caso di Amministrazione, modifica corso:

			- scenario principale  (4a): 
						4.1)   valutazione delle motivazioni che ne causerebbero la modifica
						4.2a)  amministrazione valuta positivamente le motivazioni 
						4.3a)  amministrazione informa studenti e docenti dei cambiamenti
						4.4a)  amministrazione procede effettivamente all' applicazione delle modifiche
			
			- scenario secondario: (4b):  
						4.2b)  amministrazione non ritiene valide le motivazioni 
						4.3b)  amministrazione informa ministero dell' impossibilità di procedere alla modifica

5. caso di amministrazione, cancellazione corso:

			-scenario principale   
						5.1)   amministrazione Valuta le motivazioni se non richiesto dal ministero
						5.2)   amministrazione informa preventivamente studenti e docenti 
						5.3)   amministrazione procede effettivamente alla cancellazione

caso di Amministrazione, creazione docente:
	
			- scenario principale  (6a): 
						6.1)   amministrazione valuta la candidatura 
						6.2a)  amministrazione assume il docente che possiede i requisiti necessari

			- scenario secondario  (6b):
						6.2b)  amministrazione non assume il docente che difetta dei requisiti necessari

caso di amministrazione, cancellazione docente:

			- scenario principale  (7a):
						7.1)   amministrazione valuta le motivazioni per procedere alla cancellazione
						7.2)   amministrazione valuta necessario sostituire vecchio docente
						7.3a)  amministrazione si accorda con nuovo docente
						7.4a)  amministrazione licenzia vecchio docente

			- scenario secondario  (7b):			
						7.3b)  amministrazione valuta non necessario sostituire vecchio docente
						7.4b)  amministrazione licenzia vecchio docente






	

