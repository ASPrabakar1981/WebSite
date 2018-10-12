pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps { 
               sh 'make'
            }
        }
        stage('Test'){
             steps { 
                sh 'make check'
            }
        }
        stage('Deploy') {
             steps { 
              sh 'make publish'
            }
        }
    }
}
