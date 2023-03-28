pipeline{
   agent any
  stages{
    stage('git cloning'){
      steps{
        script{
         git branch: 'main', credentialsId: 'git_id', url: 'https://github.com/jyothikaruparthi/demo_project.git'
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
  }
}
