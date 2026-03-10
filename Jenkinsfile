pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git url: 'https://github.com/ManojM1107/Internals.git',
                    branch: 'main'
            }
        }
        stage('Run Script') {
            steps {
                // Ensure Python is available in Jenkins agent
                sh 'chmod +x add.py'
                sh 'python3 add.py'
            }
        }
    }
}
