pipeline {
    agent any
    tools {
        maven: 'maven_361'
    }
    
    stages {
        stage('Initialize') {
            def MVN_HOME = tool name: 'maven_361', type: 'maven'
            def MVN = "${MVN_HOME}/bin/mvn"
        }

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
