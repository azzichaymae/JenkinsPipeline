pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/azzichaymae/JenkinsPipeline.git'
            }
        }

        stage('Compile') {
            steps {
                echo 'Compilation des classes...'
                sh 'javac HelloWorld.java Merci.java DeRien.java'
            }
        }

        stage('Run HelloWorld') {
            steps {
                echo 'Exécution HelloWorld...'
                sh 'java HelloWorld'
            }
        }

        stage('Run Merci') {
            steps {
                echo 'Exécution Merci...'
                sh 'java Merci'
            }
        }

        stage('Run DeRien') {
            steps {
                echo 'Exécution DeRien...'
                sh 'java DeRien'
            }
        }
    }

    triggers {
        cron('* * * * *')   // exécuter chaque minute (comme dans l'exercice)
    }
}
