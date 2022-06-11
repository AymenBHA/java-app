def gv
pipeline {
    agent any
    tools {
        maven "Maven"
    }
    stages {
        stage('Initialize'){
            steps{
                echo "hello"
                script {
                    gv = load "dcript.groovy"
                }
            }
        }
        stage('Build jar') {
            steps {
                echo "build jar"
                script {
                    gv.buildJar()
                }
            }
        }
        stage('Build image') {
            steps {
                echo "build image ..."
                script {
                    gv.buildImage()
                }
            }
        }
        stage('deploy') {
            steps {
                echo "deploy app ..."
                script {
                    gv.deployApp()
                }
            }
        }
     }
}
