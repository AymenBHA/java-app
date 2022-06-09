def gv
pipeline {
    agent any
    tools {
        maven 'mvn'
    }
    stages {
        stage("init"){
            steps {
                script {
                    gv.buildJar()
                }
            }
        }

        stage("build jar"){
            steps {
                script {
                    gv.buildImage()
                }
            }
        }

        stage("deploy"){
            steps {
                script {
                    gv.deployApp()
                }
            }
        }

    }
}
