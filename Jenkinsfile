pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'etape de build /w git'
                echo 'etape de build /w update git'
                sh 'python3 --version'
            }
        }
        stage('test unitaires ') {
            when {
                branch 'develop'
            }
            steps {
                echo 'etape de test unitaires'
            }
        }
        stage('test d\'integration') {
            steps {
                echo 'etape de test unitaires'
            }
        }
        stage('deploy') {
            steps {
                echo 'etape de deploiment sur env dev'
            }
        }
    }
}
