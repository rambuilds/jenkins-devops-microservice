
//SCRIPTED PIPELINE
//DECLARATIVE PIPELINE
pipeline{
	agent{
		docker{
			image='maven:3.8'
		}
	}
	stages{
		stage('build'){
			steps{
				sh 'mvn --version'
				echo 'build'
			}
		}
		stage('test'){
			steps{
				echo 'test'
			}
		}
		stage('integration test'){
			steps{
				echo 'integration test'
			}
		}
	} 
	post{
		always{
			echo 'always'
		}
		success{
			echo 'success'
		}
		failure{
			echo 'failure'
		}
	}
}
