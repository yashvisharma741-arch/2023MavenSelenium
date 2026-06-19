pipeline{
  agent any
    tools{
      maven 'Maven'
      }
    stages{
      stage('Checkout'){
        steps{
          git branch:'main', url:'https://github.com/yashvisharma741-arch/2023MavenSelenium.git'
          }
          }
       stage('Build'){
         steps{
           sh 'mvn clean package'
           }
           }
       stage('Test'){
         steps{
           sh 'mvn test'
           }
           }
            }
      post{
        success{
          echo "Open SauceDemo:https://www.saucedemo.com/"
          }
        failure{
          echo 'Failed'
          }
          }
          }
          
