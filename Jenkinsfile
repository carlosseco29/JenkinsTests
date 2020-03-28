pipeline {
  agent any
  stages {
    stage("Clone repo...") {
      steps {
        git poll: true, url: 'https://github.com/carlosseco29/JenkinsTests.git'
      }
    }
    stage("Run Hello World script") {
      steps {
        sh "./myscript.sh"
      }
    }
    stage("Exit") {
      steps {
        echo "Exiting..."
      }
    }
  }
}
