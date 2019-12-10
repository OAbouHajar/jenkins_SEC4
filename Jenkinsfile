pipeline {
    agent none
    stages {
        stage('Example Fetch') {
            steps {
                    sh 'mvn clean compile'
                    echo 'Fetch Data'
                    git url: 'https://github.com/OAbouHajar/jenkins_SEC4'
            }
        }
        stage('Example build') {
            steps {
                echo 'Build Stage'
            }
        }
    }
}










