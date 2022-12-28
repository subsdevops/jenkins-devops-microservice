//SCRIPTED

//DECLARATIVE
pipeline {
	// agent any
	// agent { docker { image 'maven:3.6.3'} }
	agent { docker { image 'node:19.3'}}
	stages {
        stage('Build') {
			steps {
	            //sh 'mvn --version'
				sh 'node --version'
				echo "Build"
			}
		}	
        stage('Test') {
			steps {
	            echo "Test"
			}
		}	
	    stage('Integration test') {
			steps {
	            echo "Integeration Test"
		    }
		}		   	
   } 
   
   post {
	   always {
		   echo 'Im awesome. I run always'
	   }
       success {
		   echo 'I run when you are successful'
	   }
	   failure {
		   echo 'I run when you fail'
	   }  
	   }
}
