![alt tag](.png)

#### Scenari


###	2.1 Studente


		Caso di studente: Iscrizione a corso
	

			scenario principale:

				1) lo studente chiede di essere iscritto ad un corso
				2) l'amministrazione chiede i documenti e verifica i requisiti dello studente
				3) L'amministrazione iscrive lo studente al corso
				4) il sistema registra lo studene iscritto
				5) studente iscritto

			Scenario alternativo	

		
				3b) requisiti non idonei
				1) studente non iscritto

			Post condizione
				Viene creato un profilo studente, con tutte le informazioni personali e gli vengono assegnate
				delle credenziali di accesso.

		Caso di studente: Cancellazione da corso

			scenario principale:

				1) lo studente chiede di essere cancellato da un corso
				2) l'amministrazione cancella studente dal corso
				3) il sistema cancella lo studente 
				4) l'utente cancellato
	

		caso di studente: Visualizzazione corsi

			scenario 

				1) lo studente chiede di visualizzare i corsi a cui è iscritto
				2) il sistema verifica che lo studente esista
				3) Utente esiste
				4) il sistema fa visualizzare i corsi 
				5) l'utente visualizza i corsi
	
			scenario alternativo

				3b) utente non esiste
				1)  l'utente non visualizza i corsi


		Caso di studente: lista esami superati

			scenario
		
				1) lo studente chiede lista degli esami superati
				2) il sistema chiede nome utente e password
				3) loggin riuscito
				4) il sistema va visualizzare esami superati
				5) studente visualizza esami superati

			scenario alternativo:
		
				3b) loggin non riuscito
				1)  password sbagliata
				2) studente non visualizza esami superati
	
			Post condizione:

				Viene stampato documento con esami superati

		
			scenario alternatio 2:
				3c) loggin non riuscito
				1) nome utente non trovato
				2) studente non visualizza esami superati 

		Caso di studente: lista esami
		
				1) lo studente chiede di visualizzare lista esami dispnibili
				2) lo studente insesciri le credenziali di autenticazione
				3) loggin riuscito
				4) lo studente visualizza gli esami disponibili.
				5) lo studente prenota un esame
				6) il sistema registra lo studente all'esame
				7) studente registrato
	
			Post condizione:
		
				viene stampata la data dell'esame.






	

