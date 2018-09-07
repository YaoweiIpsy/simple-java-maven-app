pipeline {
    stages {
        stage('Build') {
            steps {
                def version = sh ( script: "hostname" , returnStdout: true ).trim()
                sh "Build $version"
            }
        }
        stage('Test') {
            steps {
                sh "Test $version"
            }
         }
    }
}