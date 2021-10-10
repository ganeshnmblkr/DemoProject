pipeline{
	agent any
	tools {
        maven 'Maven3.8.3' 
    }

	stages{
    stage("CompileStage"){
			steps{
				  bat 'mvn clean compile'
				}
		}
		stage("Testing Stage"){
			steps{
				bat "mvn test"
			}
		}
		stage("Deploy"){
			steps{
				bat "mvn deploy"
			}
		}
	}
}
