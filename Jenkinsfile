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
                def mavenHome = tool name: 'maven_361', type: 'maven'
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
