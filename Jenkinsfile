pipeline{
  agent any
  tools{
    gradle 'Gradle'
    JDK 'jdk'
  }
  stages{
    stage('Checkout'){
      steps{
        git branch:'master',
          url:'https://github.com/Ranjana2225/gradle01.git'
      }
    }
    stage('Build'){
      steps{
        sh 'gradle build'
      }
    }
    stage('Test'){
      steps{
        sh 'gradle test'
      }
    }
    stage('Run application){
          steps{
            sh 'gradle run'
          }
        }
    }
   post{
     success{
       echo 'Build successful'
     }
     failure{
       echo 'Build failed'
     }
   }
          }          
          
          
          
      
      

      
    
