pipeline{     
	agent any     
	stages {     
		stage('build'){     
				steps{     
					sh 'ant -f build.xml -v'     
				}    
		 }     
	}
	post {   
		always{   
			archiveArtifacts artifacts: '*.jar', fingerprint: true   
		}    
	 }      
} 
 
 
