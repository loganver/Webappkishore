pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        git 'https://github.com/kishorekk12/webAppExample.git'
      }
    }

    stage('stage2') {
      steps {
        bat 'mvn install'
      }
    }

    stage('stage3') {
      steps {
        archiveArtifacts '*/*.war'
      }
    }

  }
}