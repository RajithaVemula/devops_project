pipeline {
  agent any
  stages {
    stage('stage 1') {
      steps {
        sh 'echo "hello,stage1"'
      }
    }

    stage('stage 2') {
      steps {
        sh 'echo "Hello, stage2"'
        git(url: 'https://github.com/RajithaVemula/devops_project.git', branch: 'main', poll: true)
      }
    }

  }
}