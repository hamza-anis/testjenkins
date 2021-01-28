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
<<<<<<< HEAD
        stage('tests') {
=======
        stage('test unitaires ') {
>>>>>>> develop
            when {
                branch 'release'
            }
            steps {
                echo 'etape de test unitaires'
<<<<<<< HEAD
                echo 'etape de test ti'
                echo 'etc... '
=======
                sh 'python3 index.py'
            }
        }
        stage('test d\'integration') {
            steps {
                echo 'etape de test unitaires'
                echo 'etape de test trigger'
>>>>>>> develop
            }
        }
        stage('deploy') {
            when {
                branch 'release'
            }
            steps {
<<<<<<< HEAD
                sh '''
                echo "deploying into release env"
                '''
=======
                echo 'etape de deploiment sur env dev'
>>>>>>> develop
            }
        }
    }
}
