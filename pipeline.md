Create a pipeline in Jenkins:
1. Go to Jenkins --> New Item --> "Enter Item name" --> select Pipeline tab --> Ok
in the configure pipeline add the below code :
```
pipeline {
    agent any
    stages{
        stage('stage 1'){
            steps{
                
                echo "step1"
            }
          
        }
        stage('Preparation') { // for display purposes
            steps{
                script{
               def a = 100

                echo "value is " + a
                }
            }
        }
   }
  
}
```
