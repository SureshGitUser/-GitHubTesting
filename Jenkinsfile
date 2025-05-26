pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'gradlew clean bootJar'
            }
        }
        stage('Run') {
            steps {
                bat 'java -jar build/libs/TestGitHub-0.0.1-SNAPSHOT.jar'
            }
        }
    }
}
