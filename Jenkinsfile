pipeline {
    agent any

    stages {

        stage('Compile') {
            steps {
                echo 'Compilation des classes...'
                bat 'javac HelloWorld.java Merci.java DeRien.java'
            }
        }

        stage('Run HelloWorld') {
            steps {
                bat 'java HelloWorld'
            }
        }

        stage('Run Merci') {
            steps {
                bat 'java Merci'
            }
        }

        stage('Run DeRien') {
            steps {
                bat 'java DeRien'
            }
        }
    }
}
