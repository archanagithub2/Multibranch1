pipeline{
  agent any
  
  stages{
    stage('Print Java'){
      steps{
       sh 'java -version' 
      }
    }
    
     stage('cat README'){
       when{
         branch 'source1' 
       }
      steps{
       sh 'cat README.md' 
      }
    }
    
     stage('Printing Hello'){
       when{
         branch 'source2' 
       }
      steps{
       echo 'Hello' 
      }
    }
    
     stage('Greeting'){
       when{
         branch 'source1' 
       }
      steps{
       echo 'Hello world' 
      }
    }
  }
}
