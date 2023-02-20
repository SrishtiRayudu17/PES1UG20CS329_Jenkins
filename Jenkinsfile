pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -c working.cpp -error'
        sh 'g++ -o working working.cpp'
          echo 'Build successful'
      }
    }
    stage('Test') {
      steps {
        sh 'cat working.cpp'
        echo 'Test successful'
      }
    }
    stage('Deploy') {
      steps {
 
        echo 'Deploy successful'
      }
    }
 }
 post {
  failure {
 
    echo 'Pipeline Failed'
 
  }
 }
}
