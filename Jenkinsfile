pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting Build'
                sh 'make -C main'
                echo 'Build Completed'
            }
        }
        stage('Test') {
            steps {
                echo 'Starting Testing'
                sh '/var/jenkins_home/workspace/diesha_pes2ug20cs111-1/main/hello_exec'
                echo 'Test Completed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Starting Deploy'
                echo 'Deploy Completed'
            }
        }
    }
  post {
    failure {
      echo 'Pipeline Failed'
    }
  }
}
