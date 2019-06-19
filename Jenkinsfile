pipeline {
    agent any

    tools {
        maven: 'maven_361'
    }

    stages {

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