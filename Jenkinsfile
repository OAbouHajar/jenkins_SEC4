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
            stage("Docker Compose") {
              steps {
                echo "Docker compose up"
              }
            }
            stage("Run tests") {
              steps {
                echo "Executing Firefox"
              }
            }
            stage("SQ Report") {
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
    stage("Dev") {
      steps {
        echo "Executing Dev"
      }
    }
  }
}





