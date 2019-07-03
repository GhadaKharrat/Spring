# Spring
En effet, Maven a :

copié les ressources de l'application 

compilé les sources de l'application

compilé les sources des tests

exécuté les tests sur l'application (1 test exécuté, aucune erreur)

généré un JAR de l'application

Pas mal, hein !? ;)

Vous pouvez lancer votre application Java flambant neuve :

java -cp target/mon-appli-1.0-SNAPSHOT.jar org.exemple.demo.App
Ce qui devrait vous afficher un magnifique :

Hello World!
Résumons
Dans ce chapitre, j'ai survolé rapidement la gestion de projet Java avec Apache Maven.

Voici les choses importantes à retenir :

Maven utilise une approche « convention over configuration » (ou convention plutôt que configuration en français).

L'arborescence d'un projet Maven est fixée par convention. Elle comporte :

un fichier pom.xml à la racine qui sert à décrire et configurer le projet Maven ;

un répertoire src/main/java contenant les sources de l'application ;

un répertoire src/test/java contenant les sources des tests JUnit de l'application.

Pour créer un nouveau projet Maven, vous pouvez générer l'arborescence en utilisant un archétype grâce à la commande mvn archetype:generate.

Compilez votre projet, exécutez les tests et construisez un JAR de votre application en une seule commande : mvn package. Si la compilation et tous les tests passent sans encombre, un fichier target/<artifactId>-<version>.<packaging> est généré (soit target/mon-appli-1.0-SNAPSHOT.jar dans mon exemple).