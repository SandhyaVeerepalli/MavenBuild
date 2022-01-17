pipeline{
  agent any
  
  
  stages{
    stage("Git Checkout"){
      steps{
            git credentialsId: 'github', url: 'https://github.com/SandhyaVeerepalli/MavenBuild'
           }
          }
     stage("Maven Build"){
       steps{
            sh "mvn clean package"
            sh "mv target/*.war target/MavenBuild.war"
             }
           
      }
    }
