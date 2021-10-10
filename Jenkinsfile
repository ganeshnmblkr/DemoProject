pipeline{
	agent any
	tools {
        maven 'Maven3.8.3' 
    }

	stages{
    stage("CompileStage"){
			steps{
				  sh 'mvn clean compile'
				}
		}
		stage("Testing Stage"){
			steps{
				sh "mvn test"
			}
		}
		stage("Deploy"){
			steps{
				sh "mvn deploy"
			}
		}
	}
}
