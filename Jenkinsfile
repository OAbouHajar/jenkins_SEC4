pipeline {
    agent none
    stages {
     stage('fetch') {
                steps {
                    echo "fetch Data"
    	            }
            }
        stage('Compile') {
            steps {
                echo "build Data"
                 bat 'javac "D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\src\\Student.java"'
	            }
        }
            stage('Test') {
              steps {
                echo "Test Data "
                bat 'java -cp .;"D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\all\\junit-4.13.jar";"D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\all\\hamcrest-core-1.3.jar";. org.junit.runner.JUnitCore "D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\src\\studentTest"'
              }
            }

    }
}





