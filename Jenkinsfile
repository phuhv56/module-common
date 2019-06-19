pipeline {
    agent any
    stages {

        stage ('Show pwd') {

            steps {
                sh 'pwd'
            }

        }

        stage ('Compile and Install State') {

            steps {
                sh 'mvn clean install'
            }

        }

        stage ('Build') {
            steps {
                echo 'This is step build'
            }
        }

    }
}