
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
                git clone https://github.com/Yasminemaroukk/devopsesprit.git
            }
        }
 
        stage('Affichage de la date système') {
            steps {
                // Cette étape affiche la date système
                script {
                    def date = sh(script: 'date', returnStdout: true).trim()
                    echo "La date système est : ${date}"
                }
            }
        }
    }
}
 
