pipeline {
    agent any
    tools {
        maven "Maven"
    }
    stages {
        stage('Initialize'){
            steps{
                echo "hello"
            }
        }
        stage('Build') {
            steps {
                sh 'mvn --version'
            }
        }
     }

}
