pipeline {
    agent none
  stages {
    stage('Docker pull') {
        agent any
      steps {
          sh 'docker pull aritzmetal/todoapp:v4'
      }
    }
    stage('Docker Run') {
        agent any
      steps {
            sh "docker run -p 82:3000 --name tod aritzmetal/todoapp:v4"
        }
    }
}
}
