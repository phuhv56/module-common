pipeline {
    agent any
    
    stages {

        stage ('Show pwd') {

            steps {
                sh 'pwd'
            }

        }

        stage ('Compile and Install State') {
            def mavenHome = tool name: 'maven_361', type: 'maven'
            steps {
                sh '${mavenHome}/bin/mvn clean install'
            }

        }

        stage ('Build') {
            steps {
                echo 'This is step build'
            }
        }

    }
}
