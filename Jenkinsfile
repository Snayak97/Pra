@Library('Shared') _
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script{
                    hello()
                }
            }
        }
       stage('cleen workspace') {
            steps {
                deleteDir()
                echo 'Workspace cleaned successfully'
            }
        }
        stage('clone code') {
            steps {
                script{
                    clone("https://github.com/Snayak97/Pra.git","main")
                }
            }
        }
    }
}
