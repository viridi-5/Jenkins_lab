pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compiling app.cpp into executable pes1ug22am064-1'
                // This command compiles the C++ file (ensure the file is named app.cpp)
                sh 'g++ -o pes1ug22am064-1 pes1ug22am064.cpp'
            }
        }
        stage('Test') {
            steps {
                echo 'Executing pes1ug22am064-1'
                // This command runs the compiled binary and prints its output
                sh './pes1ug22am064-1'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying pes1ug22am064-1'
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
