pipeline{
  tools{
    jdk 'my_jdk'
    mvn 'my_maven'
  }
  agent none
  stages{
    stage('checkout'){
      agent any
      steps{
        git 'https://github.com/BlackWidow23/JenkinsDocs.git'
      }
    }
    stage('compile'){
      agent any
      steps{
        sh 'mvn compile'
      }
    }
    stage('unittest'){
      agent any
      steps{
        sh 'mvn test'
      }
    }
  }
}
