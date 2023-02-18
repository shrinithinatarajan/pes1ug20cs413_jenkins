pipeline{
	agent any
	stages  {
		stage('Build') {
			steps{
				sh 'g++ -c pes1ug20cs413.cpp'
				sh 'g++ -o pes1ug20cs413 pes1ug20cs413.cpp'
				echo 'Build was successful'
			}
		}
		stage('Test") {
			steps {
				sh './pes1ug20cs413'
				echo 'Test was successful'
			}
		}
		stage('Deploy') {
			steps {
				echo 'Deployed'
			}
		}
	}
	post{
		failure{
			echo 'Pipelining unsuccessful'
		}
	}
}
