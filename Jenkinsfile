pipeline{
	agent any
	stages{
    stage("CompileStage"){
			steps{
				maven(maven :'Maven3.8.3'){
				  sh 'mvn clean compile'
				}
			}
		}
		stage("Testing Stage"){
			steps{
				maven(maven :'Maven3.8.3'){
				sh "mvn test"
				}
			}
		}
		stage("Deploy"){
			steps{
				maven(maven :'Maven3.8.3'){
				sh "mvn deploy"
				}
			}
		}
	}
}
