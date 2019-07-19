pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh "mvn clean"
            }
        }
        stage('--test--') {
            steps {
                sh "mvn -Dmaven.test.skip=true"
            }
        
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }
    }
}
}
