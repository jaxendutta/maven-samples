pipeline {
  agent any
  tools { 
      maven 'Maven 3.9.9' 
      jdk 'Java 21' 
  }
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/jaxendutta/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}