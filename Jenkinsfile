pipeline {
    agent any
    
    stages {
        stage('Initialize') {
            steps {
                def MVN_HOME = tool name: 'maven_361', type: 'maven'
                def MVN = "${MVN_HOME}/bin/mvn"
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
