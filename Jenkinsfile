pipeline {
    agent none
    stages {
        stage('Compile') {
            steps {
                echo "build Data"
                 bat 'javac -cp .;"D:\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\all\\junit-4.13.jar" studentTest.java'
	            }
        }
            stage('Test') {
              steps {
                echo "Test Data "
                sh 'java -cp .;"D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\all\\junit-4.13.jar";"D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\all\\hamcrest-core-1.3.jar";. org.junit.runner.JUnitCore "D:\\IT Carlow\\Year4\\Soft Eng\\jenkins\\studentAtt\\src\\studentTest"'
              }
            }

    }
}





