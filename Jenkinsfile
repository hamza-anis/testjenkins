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
        stage('Build Deploy Code') {
            when {
                branch 'develop'
            }
            steps {
                sh '''
                echo "test condition only develop branch"
                '''
                sh '''
                echo "Building code from develop"
                '''
                sh '''
                echo "Deploying code from develop 2 "
                '''
            }
        }
        stage('test') {
            steps {
                echo 'etape de test /w git toto'
            }
        }
        stage('deploy') {
            steps {
                echo 'etape de deploiment /w git updated'
            }
        }
    }
}
