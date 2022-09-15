
### User Requirements Specification Document
##### DIBRIS – Università di Genova. Scuola Politecnica, Software Engineering Course 80154


**VERSION : 10.2**

**Authors**  
Simone Schiano <br>
Giacomo Cattozzo <br>
Jandry Vicente

**REVISION HISTORY**

| Version     | Date       | Authors      | Notes        |
| ----------- | ---------- | -----------  | -----------  |
| 10.2.1 | 15/09/2022  | Simone, Giacomo, Jandry | Aggiornamento di sicurezza  |
| 10.2.2 | 21/09/2022  | Simone, Giacomo, Jandry | Correzione bug |
| 10.2.3 | 28/09/2022  | Simone, Giacomo, Jandry | Aggiornamento di sicurezza  |
| 11.0.1 | 15/09/2022  | Simone, Giacomo, Jandry | Nuova versione del software |

# Table of Contents

1. [Introduction](#p1)
	1. [Document Scope](#sp1.1)
	2. [Definitios and Acronym](#sp1.2) 
	3. [References](#sp1.3)
2. [System Description](#p2)
	1. [Context and Motivation](#sp2.1)
	2. [Project Objectives](#sp2.2)
3. [Requirement](#p3)
 	1. [Stakeholders](#sp3.1)
 	2. [Functional Requirements](#sp3.2)
 	3. [Non-Functional Requirements](#sp3.3)
  
  

<a name="p1"></a>

## 1. Introduction

Ci è stato richiesto un software con il quale i professori e gli studenti potessero esaminare e interagire con vari aspetti di corsi e esami.

<a name="sp1.1"></a>

### 1.1 Document Scope
	Tramite l’applicazione
	il docente potrà visualizzare i corsi di cui è docente, per ogni corso indire
	un esame, visualizzare la lista degli studenti iscritti all’esame, e per ogni
	studente iscritto registrare un votazione (0-30).
	Uno studente invece potrà visualizzare: la lista dei corsi a cui è iscritto,
	la lista dei corsi superati con relativa valutazione e per ogni esame la lista
	degli esami a cui si può iscrivere. Inoltre si può iscrivere a un esame di ogni
	corso a cui è iscritto e che non ha ancora superato.


<a name="sp1.2"></a>

### 1.2 Definitios and Acronym


| Acronym				| Definition | 
| ------------------------------------- | ----------- | 
| E.C.D.S.                                  | Esami e Corsi per Docenti e Studenti |

<a name="sp1.3"></a>

### 1.3 References 
	assistenza email segreteria infosegreteria@gmail.it
	www.assistenzasitoweb.it
	Autore del software
	
<a name="p2"></a>

## 2. System Description

<a name="sp2.15"></a>

Il software è scritto in linguaggio Python. Il Software inoltre si divide in vari classi tramite le quali i docenti possono verificare i propri corsi e aggiungere esami e risultati mentre gli studenti possono verificare i corsi a cui appartengono, possono isciversi ad esami e possono vederne i risutati.

### 2.1 Context and Motivation
	Ci è stato chiesto di creare un software per la gestione degli esami e la registrazione dei voti che possa essere utile per docenti e studenti.
	
<a name="sp2.2"></a>

### 2.2 Project Obectives 
	Fare in modo che il docente disponga di una lista in cui il docente può visualizzare i propri corsi, programmare un esame, lista di studenti iscritti a esame, voto per ogni studente da 0 a 30.
	Lo studente avrà accesso ad un lista di corsi a cui è iscritto, lista esami superati con valutazione e lista di esami a cui si può iscrivere.
	
	

<a name="p3"></a>

## 3. Requirements
	

| Priorità | Significato | 
| --------------- | ----------- | 
| M | **Mandatory:**   |
| D | **Desiderable:** |
| O | **Optional:**    |
| E | **future Enhancement:** |

<a name="sp3.1"></a>

### 3.1 Stakeholders
-UNIVERSITA' <br>
-DOCENTI <br>
-STUDENTI <br>
-TECNICO INFORMATICO

<a name="sp3.2"></a>
### 3.2 Functional Requirements 

| ID | Descrizione | Priorità |
| --------------- | ----------- | ---------- | 
| 1.0 |  Programma per Windows e Mac |M|
| 2.0 |  Programma per Linux |D|
| 3.0 |  Applicazione per IOS e ANDROID |E|
| 4.0 |  Credenziali di accesso per docenti e studenti |M|



<a name="sp3.3"></a>
### 3.3 Non-Functional Requirements 
 
| ID | Descrizione | Priorità |
| --------------- | ----------- | ---------- | 
| 1.0 | Performance del software |E|
| 2.0 | Usabilità |O|
| 3.0 | Struttura del software |O|
