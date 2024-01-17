pipeline {
    agent none

    stages {
        stage('Hello') {
            agent { label 'robotfw' }
            steps {
                container('robotfw') {
                    echo 'Hello World'
                    echo 'Test auto build master'
                    sh 'python3 --version'
                }
            }
        }
    }
}
