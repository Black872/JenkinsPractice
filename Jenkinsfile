pipeline {
    agent {
	label 'master'
	}
    options {
	buildDiscarder(logRotator(numToKeepStr: '5', artifactNumToKeepStr: '6'))
	timestamps()
	}
	
    stages {
        stage ('First step') {
            steps {
                echo "Start"
		sh 'ssh jenkins@10.202.2.48 \'hostname\''
                echo "Doing something.."
                echo "End"

            }

        }
    }
}
