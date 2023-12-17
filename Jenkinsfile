pipeline{
agent any 
tools{
  maven 'Maven 3_6_3'
}
  
  stages {
    stage('checkout'){
      steps{
        git 'https://github.com/ganate34/testmedemo.git
      }
    }
    stage('Build'){
      steps{
        sh 'mvn install' 
      }
    }
    stage('Test'){
      steps{
        sh 'mvn test'
      }
    }
  }
}
