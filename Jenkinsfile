pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'etape de build'
                echo 'SHOW PY version'
                sh 'python3 --version'
            }
        }
        stage('test unitaires ') {
            when {
                branch 'release'
            }
            steps {
                echo 'etape de test unitaires'
                sh 'python3 index.py'
            }
        }
        stage('test d\'integration') {
            steps {
                echo 'etape de test unitaires'
                echo 'etape de test trigger release'
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
