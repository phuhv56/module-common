pipeline {
    agent any
    
    stages {
        stage('Initialize') {
            steps {
                script {
                    def MVN_HOME = tool name: 'maven_361', type: 'maven'
                    sh '${MVN_HOME}/bin/mvn clean install'
                }
            }
        }

        stage ('Build') {
            steps {
                echo 'This is step build'
            }
        }

    }
}
