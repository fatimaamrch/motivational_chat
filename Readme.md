# Chat Motivant - API & Application Spring Boot

Une application inspirante pour les employés d'une entreprise. Ce projet inclut une API Spring Boot qui fournit des citations inspirantes et une application Spring Boot permettant aux employés de discuter avec l'API et d'enregistrer leurs conversations.

## Contexte

Récemment, les employés manquent de motivation. L'idée est de créer un chat qui les aide à se sentir mieux en leur offrant des citations inspirantes et en enregistrant leurs conversations.

## Objectifs

1. Développer une API Spring Boot qui renvoie une citation inspirante aléatoire.
2. Créer une application Spring Boot qui permet aux employés d'interagir avec cette API, d'enregistrer leurs conversations et de voir un historique de celles-ci.

## Technologies

- **Java 11+**
- **Spring Boot** (pour l'API et l'application)
- **MySQL**
- **Maven** (gestion des dépendances et construction des projets)
- **RestTemplate** (pour appeler l'API depuis l'application de chat)

## Prérequis

Avant de commencer, assurez-vous d'avoir installé :

- **JDK 11+**
- **Maven**
- **MySQL** ou une autre base de données relationnelle

## Installation

1. Clonez ce repository.

   ```bash
   git clone https://github.com/fatimaamrch/motivational_chat.git
   cd motivational_chat
   
   
2. Configurez votre base de données.

	Créez une base de données MySQL et ajoutez la configuration dans le fichier application.properties de chaque projet :


		spring.datasource.url=jdbc:mysql://localhost:3306/motivational_chat_db
		spring.datasource.username=root
		spring.datasource.password=votre_mot_de_passe
		
3. Lancez l'API Spring Boot.


	L'API sera disponible à l'adresse : http://localhost:8081/api/quotes

4. Lancez l'application de chat.

	L'application sera disponible à l'adresse : http://localhost:8080
	
	 http://localhost:8080/chat : accès au chat
	 http://localhost:8080/sendMessage : affichage de la citation lors de l'envoie du message de l'utilisateur
	 http://localhost:8080/discussion : affichage de l'historique de discussions 
	  
	