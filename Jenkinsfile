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
}
