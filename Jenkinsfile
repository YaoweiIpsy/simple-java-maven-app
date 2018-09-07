pipeline {
    agent any
    stages {
        stage('somestage') {
            steps {
                script {
                    def version = sh (
                        script: "hostname",
                        returnStdout: true
                    ).trim()
                    sh "echo Building project in version: $version"

                }
            }
        }
        stage('test') {
            echo("------ ${version}")
        }

    }
}