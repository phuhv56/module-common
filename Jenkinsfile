pipeline {
    agent any
    tools {
        maven: 'maven_361'
    }
    stages {

        stage ('Show pwd') {

            steps {
                sh 'pwd'
            }

        }

        stage ('Compile and Install State') {
            
            steps {
                sh '${MAVEN_HOME}/bin/mvn clean install'
            }

        }

        stage ('Build') {
            steps {
                echo 'This is step build'
            }
        }

    }
}
