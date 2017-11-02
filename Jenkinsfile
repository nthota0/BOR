pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/nthota0/MavenRepo_New.git', branch: 'master', poll: true)
      }
    }
    stage('BUILD') {
      steps {
        sh 'mvn clean compile package'
      }
    }
    stage('upload') {
      steps {
        sh 'mvn deploy'
      }
    }
  }
}