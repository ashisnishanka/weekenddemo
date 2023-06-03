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
		  stage("test"){
	    steps{
		 sh 'mvn test'
		}
		}
		   stage("package"){
	    steps{
		 sh 'mvn1 package1'
		}
		}
		 stage("deploy"){
	    steps{
		  echo "my deployment is success"
		}
		}
	  }
	}
