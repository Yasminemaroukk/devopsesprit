pipeline {
    agent any
    triggers {
        // Configuration du déclenchement du pipeline lorsqu'un push est détecté dans le référentiel Git
        pollSCM 'H/5 * * * *'
    }
    stages {
        stage('Récupération du code source') {
            steps {
                // Cette étape clone le référentiel Git
                echo "hello"
            }
        }

        stage('Affichage de la date système') {
            steps {
                // Cette étape affiche la date système
                
                    
                echo "La date système est "
                
            }
        }
    }
}
