pipeline {
    agent none
    stages {
        stage('Fetch') {
            steps {
                    echo "Fetch Data"
                    bat "git fetch origin"
                    bat "cd jenkins_SEC4"
            }
        }
        stage('Compile') {
            steps {
                echo "build Data"
                bat 'javac "src\\Student.java"'
	            }
        }
            stage('Test') {
              steps {
                echo "Test Data "
                bat 'java -cp "all\\junit-4.13.jar";"all\\hamcrest-core-1.3.jar";. org.junit.runner.JUnitCore "src\\studentTest"'
              }
            }

    }
}





