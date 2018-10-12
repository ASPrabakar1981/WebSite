pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
                withMaven(maven : 'maven_3.5.4')
				{
					sh 'mvn clean build'
				}
            }
        }
        stage('Test'){
             steps { 
                withMaven(maven : 'maven_3.5.4')
				{
					sh 'mvn test'
				}
            }
        }
        stage('Deploy') {
             steps { 
                withMaven(maven : 'maven_3.5.4')
				{
					sh 'mvn deploy'
				}
            }
        }
    }
}
