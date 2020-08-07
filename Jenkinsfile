pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/jeromewinifred/git2', branch: 'master')
      }
    }

    stage('Test') {
      steps {
        echo 'Going through the Test Stage'
      }
    }

    stage('Deploy') {
      steps {
        sh '''javac Hello.java
java Hello'''
      }
    }

  }
}