pipeline{
	agent any
	
	tools{
	    maven 'maven3'
	}
	
	stages{
		stage('pmd'){
			steps{
				sh "mvn pmd:pmd"
			}
			
			post{
				always{
					pmd(canRunOnFailed:true, pattern:'**/target/pmd.xml')		
				}
			}
		
		}
	}
}
