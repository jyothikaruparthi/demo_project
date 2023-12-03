
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
    stage('unit test'){
      steps{
        script{
          sh 'mvn test'
        }
      }
    }
    stage('intigration test'){
      steps{
        script{
          sh 'mvn verify'
        }
      }
    }
  }
}
