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
        stage('tests') {
            when {
                branch 'release'
            }
            steps {
                echo 'etape de test unitaires'
                echo 'etape de test ti'
                echo 'etc... '
            }
        }
        stage('deploy') {
            when {
                branch 'release'
            }
            steps {
                sh '''
                echo "deploying into release env"
                '''
            }
        }
    }
}
