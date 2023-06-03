pipeline{
 tools{
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
     agent any
	  
	  stages{
	  
	  stage("checkout"){
	   steps{
	   git credentialsId: 'github', url: 'https://github.com/ashisnishanka/weekenddemo.git'
	   }
	                  }
	
	   stage("compile"){
	    steps{
		 sh 'mvn compile'
		}
		}
		  
	   stage("package"){
	    steps{
		 sh 'mvn package'
		}
		}
		 stage("deploy"){
	    steps{
		  echo "my deployment is success"
		}
		}
	  }
	}
