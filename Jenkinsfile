pipeline {
  agent any 
  stages {
    stage('Clone Code') {
      steps {
        echo 'Cloning Code...'
      }
    }
    stage('Run PHP') {
      steps {
        sh 'php index.php'
      }
    }
  }
  post {
    success {
      mail to: 'madhura63644@gmail.com',
        from: 'madhura63644@gmail.com',
        subject: 'Jenkins Build Success',
        body: 'Deployment Successfully'
    }
    failure {
      mail to: 'madhura63644@gmail.com',
        from: 'madhura63644@gmail.com',
        subject: 'Jenkins Build Failed',
        body: 'Deployment Failed'
    }
  }             
}
