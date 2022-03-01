pipeline {
    agent none
  stages {
    stage("clean") {
      steps {
        echo "Executing Build"
      }
    }
    stage("init") {
      steps {
        echo "Executing Build"
      }
    }
    stage("lint") {
      steps {
        echo "Executing Build"
      }
    }
    stage("generate") {
      steps {
        echo "Executing Build"
      }
    } //generate
    stage ("Parallel Builds") {
      parallel {
        stage("stream helm") {
          stages {
            stage("image") {
              steps {
                echo "Executing image"
              }
            }
            stage("package") {
              steps {
                echo "Executing image"
              }
            }
            stage("helm lock") {
              steps {
                echo "Executing helm"
              }
            }
            stage("helm") {
              steps {
                echo "Executing helm"
              }
            }
            stage("helm test") {
              steps {
                echo "Executing helm test"
              }
            }

          }
        } //stages stream 1
        stage("stream testing") {
          stages {
            stage("Docker Compose") {
              steps {
                echo "Docker compose up"
              }
            }
            stage("Tests") {
              steps {
                echo "Executing Tests"
              }
            }
            stage("SQ") {
              steps {
                echo "Executing SQ"
              }
            }
          }
        }
      } //stages stream 2
    }//parrelle
    stage("after all") {
      steps {
        echo "Executing Dev"
      }
    }
  }
}





