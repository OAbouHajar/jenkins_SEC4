pipeline {
    agent none
    stages {
        stage('Fetch') {
            steps {
                    echo "git fetch origin"

            }
        }
        stage('Compile') {
            steps {
                echo "build Data"
                //sh 'javac "src\\Student.java"'
	            }
        }
            stage('Test') {
              steps {
                echo "Test Data "
                //sh 'java -cp "all\\junit-4.13.jar";"all\\hamcrest-core-1.3.jar";. org.junit.runner.JUnitCore "src\\studentTest"'
              }
            }

    }
}





