pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(poll: true, url: 'https://github.com/padmapv/SCM.git', branch: 'master')
      }
    }
    stage('BUILD') {
      steps {
        sh 'mvn clean compile package'
      }
    }
  }
}