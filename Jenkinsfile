 pipeline{
     agent any 
     stages{
         stage("A"){
             steps{
                 echo "========executing A========"
             }}

         stage("SCript"){
          sh '''pwd 
                ls
          calender '''
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
