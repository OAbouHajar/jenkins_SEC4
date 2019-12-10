Jenkinsfile (Declarative Pipeline)
pipeline {
    agent none
    stages {
        stage('Example Build') {
            steps {
                    sh 'mvn clean compile'
                    echo 'Fetch Data'
                    git url: 'https://github.com/OAbouHajar/jenkins_SEC4'
            }
        }
        stage('Example build') {
            steps {
                echo 'Build Stage'
                sh 'java -version'
            }
        }
    }
}










