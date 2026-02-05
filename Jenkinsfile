pipeline {
    agent any
    tools {
        jdk 'JDK17'
    }
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/atharvkolekar190/Prac6_DevO.git'
            }
        }

        stage('Compile Java') {
            steps {
                bat '''
                    javac Hello.java
                '''
            }
        }

        stage('Run Program') {
            steps {
                bat '''
                    java Hello
                '''
            }
        }
    }
}
