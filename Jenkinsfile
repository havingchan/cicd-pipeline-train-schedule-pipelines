pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running build automation master...'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
    // stage('Test') {
    //   steps {
    //     echo 'Testing..'
    //   }
    // }
    // stage('Deploy') {
    //   steps {
    //     echo 'Deploying....'
    //   }
    }
  }
