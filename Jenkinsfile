pipeline {
    agent none
    stages {
        stage('Fetch') {
            steps {
                    echo "Fetch Data"
                    bat "git fetch origin"
            }
        }
        stage('Compile') {
            steps {
                echo "build Data"
                bat "cls"
                bat 'javac "D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\src\\*.java" '
	            }
        }
            stage('Test') {
              steps {
                echo "Test Data"
                bat 'java -cp "D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\all\\junit-4.13.jar";"D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\all\\hamcrest-core-1.3.jar";. org.junit.runner.JUnitCore "D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\srcstudentTest"'
              }
            }

    }
}





