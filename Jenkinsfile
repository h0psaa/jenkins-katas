pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        sh 'echo "hello world"'
      }
    }

    stage('Build app') {
      steps {
        sh 'ci/build-app.sh'
      }
    }

    stage('Archive') {
      steps {
        archiveArtifacts 'app/build/libs/'
      }
    }

  }
}