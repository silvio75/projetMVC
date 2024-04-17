pipeline {
    agent any
    
    environment {
        // Définir le chemin vers Maven dans votre système Windows
        MAVEN_HOME = 'C:\\apache-maven-3.5.4'
        // Ajouter Maven au PATH
        PATH = "${env.PATH};${MAVEN_HOME}\\bin"
    }

    stages {
        stage('Build') {
            steps {
                // Nettoyer et installer les dépendances du projet
                bat "${MAVEN_HOME}\\bin\\mvn clean install"
            }
        }

    }
}
