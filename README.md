# CI-CD-PIPILINE-WITH-AWS
Dans ce tutoriel, vous créerez un pipeline de livraison continue pour une application web simple

# Architecture de l'application
Le diagramme ci-dessous représente, visuellement, les services utilisés au cours de ce tutoriel et la manière dont ceux-ci sont connectés. Cette application utilise GitHub, AWS Elastic Beanstalk, AWS CodeBuild et AWS CodePipeline comme décrit ci-dessous.

Tout au long du tutoriel, nous reviendrons en détail sur les services et vous indiquerons les ressources permettant de vous familiariser avec eux.

![image](https://user-images.githubusercontent.com/44079323/210100426-8c4a66a5-0cb7-4376-ac33-e7ef7147f6f1.png)

# Implémentation
## FORK du referentiel de prise en main

1- Dans un nouvel onglet de navigateur, accédez à GitHub et assurez-vous d'être connecté à votre compte.

2- Dans le même onglet, ouvrez le référentiel aws-elastic-beanstalk-express-js-sample.

3- Cliquez sur le bouton blanc « Fork » dans l'angle supérieur droit de l'écran. Vous êtes alors invité à indiquer où vous souhaitez effectuer le fork du référentiel.

4- Cliquez sur votre compte. Au bout de quelques secondes, votre navigateur affiche une copie du référentiel sur votre compte.

# Concepts clés
### Service AWS Elastic Beanstalk 

qui facilite le déploiement de votre application sur AWS Il vous suffit de charger votre code pour que Elastic Beanstalk déploie votre application, la gère et la mette à l'échelle.

### Environnement 

Collection de ressources AWS fournies par Elastic Beanstalk pour permettre l'exécution de votre application.

### Instance EC2 

Serveur virtuel dans le cloud. Elastic Beanstalk alloue une ou plusieurs instances Amazon EC2 lors de la création d'un environnement.

### Serveur web 

Logiciel qui utilise le protocole HTTP pour diffuser du contenu sur Internet. Il permet de stocker, traiter et diffuser des pages web.

### Plateforme Combinaison d'un système d'exploitation, d'un environnement d'exécution de langage de programmation, d'un serveur web, d'un serveur d'applications et de composants Elastic Beanstalk. Votre application s'exécute à l'aide des composants fournis par une plateforme.

## Concepts clés aws codebluid
Processus de génération Processus qui convertit les fichiers de code source en un artefact logiciel exécutable. Il peut comprendre les étapes suivantes : compilation du code source, exécution de tests et empaquetage du logiciel en vue de son déploiement.

## Intégration continue

Méthode de développement de logiciel consistant à envoyer régulièrement les modifications à un référentiel hébergé, suite à quoi des opérations de création et de test sont automatiquement menées.

## Environnement de génération

Regroupe le système d'exploitation, l'environnement d'exécution du langage de programmation et les outils que CodeBuild utilise pour exécuter une génération.

## Buildspec

Collection de commandes de génération et de paramètres connexes, au format YAML, que CodeBuild utilise pour exécuter une génération.

## Projet de génération

Inclut des informations sur le mode d'exécution d'une génération, notamment l'emplacement du code source, l'environnement de génération à utiliser, les commandes de génération à exécuter et l'emplacement de stockage de la sortie de génération.

## Protocole ouvert OAuth

pour obtenir une autorisation sécurisée. OAuth vous permet de connecter votre compte GitHub à des applications tierces, notamment AWS CodeBuild.
