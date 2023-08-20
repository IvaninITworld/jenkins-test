pipeline {
    agent { docker "python:3.10" }
    environment {
        USER_NAME = credentials("USER_NAME")
        PASSWORD = credentials("PASSWORD")
    }
    stages {
        stage("run") {
            steps {
                echo 'run python'
                sh 'python hello.py $USER_NAME $PASSWORD'
            }
        }
    }
}
