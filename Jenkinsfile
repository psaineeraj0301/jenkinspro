pipeline {
    agent any 
    stages {
        stage('Static Analysis') {
            steps {
                echo 'Run the static analysis to the code' 
            }
        }
        stage('Compile') {
            steps {
                echo 'Compile the source code' 
            }
        }
        stage('Security Check') {
            steps {
                echo 'Run the security check against the application' 
            }
        }
        stage('Run Unit Tests') {
            steps {
                echo 'Run unit tests from the source code' 
            }
        }
        stage('Run Integration Tests') {
            steps {
                echo 'Run only crucial integration tests from the source code' 
            }
        }
        stage('Publish Artifacts') {
            steps {
                echo 'Save the assemblies generated from the compilation' 
            }
        }
    }
    post {
        success {
            emailext body: 'A Test EMail',
            subject: 'Jenkins Test EMail',
            to: 'saineeraj0307@gmail.com'
        }
        always {
            emailext body: 'A Test EMail',
            subject: 'Jenkins Test EMail',
            to: 'saineeraj0307@gmail.com'
        }
    }
}

