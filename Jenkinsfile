
pipeline{
  agent any
  stages{
    stage('cloning'){
      steps{
        script{
          git branch: 'main', credentialsId: 'token-2', url: 'https://github.com/jyothikaruparthi/demo_project.git'
        }
      }
    }
  }
}
