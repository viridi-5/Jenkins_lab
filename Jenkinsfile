pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Compile the .cpp file using a shell script
                    sh 'g++ -o pes1ug22am064-1 hello.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Print output of the compiled .cpp file
                    sh './pes1ug22am064-1'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Deployment steps, if any (e.g., pushing to a server, etc.)
                    echo 'Deploying application...'
                }
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
