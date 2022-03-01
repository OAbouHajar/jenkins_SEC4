pipeline {
    agent none
  stages {
    stage("Build") {
      steps {
        echo "Executing Build"
      }
    }
    stage ("Parallel Builds") {
      parallel {
        stage("stream1") {
          stages {
            stage("JUnit") {
              steps {
                echo "Executing JUnit"
                sh "echo test"
              }
            }
            stage("Firefox") {
              steps {
                echo "Executing Firefox"
              }
            }
          }
        }
        stage("stream2") {
          stages {
            stage("DBUnit") {
              steps {
                echo "Executing DBUnit"
              }
            }
            stage("Edge") {
              steps {
                echo "Executing Edge"
              }
            }
          }
        }
      }
    }
  }
}





