pipeline {
    agent any
   stages {
      stage('Checkout'){
                           steps{
                                                  checkout scm
                                 }
                            }
       
       //building the web-app
   stage('Build web-service'){
                steps{
                                        sh 'mvn -f /home/robot/workspace/accomodation-jenkins/hoteljsf clean install'
                                   }
                          }
        //building the web-service
         stage('Build web-service'){
                steps{
                                        sh 'mvn -f /home/robot/workspace/accomodation-jenkins clean install'
                                   }
                          }
    
    }
}
