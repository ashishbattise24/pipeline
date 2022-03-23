pipeline{
   agent any

    stages{

       stage('build image'){
         steps{
            script{
                  
                  docker.withRegistry('', 'dockerhub'){
                  
                    def image = docker.build('battiseashish24/learning-pipeline-nodejs:l.0') 
                        image.push() 
                  }
            }

         }
       }

    }
}
