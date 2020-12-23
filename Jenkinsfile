pipeline {
        agent any
        tools {
        maven 'maven3.6.3'
        }
        stages {
        stage("Checkout") {
                steps {
                git url: 'https://github.com/jamesmthornton68/5.2_BuildingCI_PipelinesInJenkins.git'

                }
        }
        stage('Build') {
                steps {
                sh "mvn compile"

                }
        }

        stage("Unit test") {
                steps {
                sh "mvn test"
                }
       	}
	}
}




