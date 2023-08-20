pipeline {
    agent { docker "python:3.10" }
    stages {
        stage("run") {
            steps {
                echo 'run python'
                sh 'python hello.py'
            }
        }
    }
}
