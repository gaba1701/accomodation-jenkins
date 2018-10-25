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
       
        //deploy the artifacts on glassfish
         stage('Build web-service'){
                steps{
                                        sh 'asadmin deploy --force=true /home/robot/workspace/accomodation-jenkin'
                    ///home/robot/.jenkins/workspace/test-jenkins-pipeline/hoteljsf
                    
                                   }
                          }
       
               //deploy clean DB
         stage('clean DB'){
                steps{
                                        sh 'psql -h localhost -U /home/robot/workspace/accomodation-jenkin'
                    ///home/robot/.jenkins/workspace/test-jenkins-pipeline/hoteljsf
                    
                                   }
                          }
    
    }
}
