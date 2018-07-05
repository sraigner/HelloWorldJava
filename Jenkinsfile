pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'mvn install'
                sh 'java -jar gs-maven-0.1.0.jar'
            }
        }
    }
}
