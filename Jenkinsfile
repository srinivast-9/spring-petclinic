
pipeline{
	agent {label 'master'}
	tools{ maven 'M3'}
	stages{
		stage('Checkout'){
			steps{
				git 'url'
			}
		}
		stage(' Build') {
			steps {
				sh 'mvn clean compile'
			}
		}
		stage(' Test') {
			steps {
				sh 'mvn test'
			}
		}
					
	}
}
