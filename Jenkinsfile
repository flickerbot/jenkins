 pipeline{
     agent any 
     stages{
         stage("A"){
             steps{
                 echo "========executing A========"
                 input 'do you wanna continue '
             }}

         stage("SCript"){
        steps{  sh '''pwd 
                ls
                     '''
             
           } 
        }

                  }
         


     
     post{
         always{
             echo "========always========"
         }
         success{
             echo "========pipeline executed successfully ========"
         }
         failure{
             echo "========pipeline execution failed========"
         }
     }
 }
