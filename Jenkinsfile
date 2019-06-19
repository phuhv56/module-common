pipeline {
    agent any
    
    stages {
        stage('Initialize') {
            steps {
                script {
                    echo env.BRANCH_NAME
                    def MVN_HOME = tool name: 'maven_361', type: 'maven'
                    echo MVN_HOME
                    sh "${MVN_HOME}/bin/mvn clean install"
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
