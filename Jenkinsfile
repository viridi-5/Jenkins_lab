pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compiling app.cpp into executable YOUR_SRN-1'
                // This command compiles the C++ file (ensure the file is named app.cpp)
                sh 'g++ -o YOUR_SRN-1 app.cpp'
            }
        }
        stage('Test') {
            steps {
                echo 'Executing YOUR_SRN-1'
                // This command runs the compiled binary and prints its output
                sh './YOUR_SRN-1'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying YOUR_SRN-1'
                // Simulate a deploy step (customize as needed)
                sh 'echo "Deployment step completed"'
            }
        }
    }

    post {
        failure {
            echo 'pipeline failed'
        }
    }
}
