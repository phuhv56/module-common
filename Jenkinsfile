pipeline {
    agent any
    
    stages {

        stage ('Show pwd') {

            steps {
                sh 'pwd'
            }

        }

        stage ('Compile and Install State') {
            
            enviroment {
                MAVEN_HOME = tool name: 'maven_361', type: 'maven'
            }
            
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
