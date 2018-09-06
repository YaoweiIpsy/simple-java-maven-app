pipeline {
    stages {
        stage('Build') {
            def version = sh ( script: "hostname" , returnStdout: true ).trim()
            sh "Build $version"

        }
        stage('Test') {
            sh "Test $version"
         }
    }
}