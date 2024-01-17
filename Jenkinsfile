pipeline {
    agent none

    stages {
        stage('Hello') {
            agent { label 'robotfw' }
            steps {
                container('robotfw') {
                    echo 'Hello World'
                    sh 'python3 --version'
                }
            }
        }
    }
}
