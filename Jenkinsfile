pipeline{
    agent any
    stages {
        stage("build"){
            steps {
                echo "etape de build /w git"
                echo "etape de build /w update git"
                sh "python3 --version"
            }
        }
        stage("test"){
            steps {
                echo "etape de test /w git tata"
            }
        }
        stage("deploy"){
            steps {
                echo "etape de deploiment /w git updated"
            }
        }
    }
}
