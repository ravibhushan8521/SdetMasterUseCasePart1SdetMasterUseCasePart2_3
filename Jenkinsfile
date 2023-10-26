pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                dir("Krissel__RestfulAndSoapWS") {
		bat "mvn clean"
	}
            }
        }
        stage('Compile') {
            steps {
	dir("Krissel__RestfulAndSoapWS") {
		bat "mvn compile"
	}
            }
        }
        stage('Test') {
            steps {
	dir("Krissel__RestfulAndSoapWS") {
		bat "mvn test"
	}
            }
        }
        stage('Result') {
            steps {
                echo "Result"
            }
        }
    }
}