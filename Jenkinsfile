pipeline{
  agent any
  stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS340 PES2UG20CS340.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS000'
    }
  }

  stage('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
  }

  post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
