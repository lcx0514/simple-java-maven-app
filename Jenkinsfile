pipeline {
	agent {
		docker {
			image 'maven:3.3.3'
			args '-v D:\WorkSpace\.m2:/root/.m2'
		}
	}
	stages {
		stage('Build') {
			steps {
				sh 'mvn -B -DskipTests clean package'
			}
		}
	}
}