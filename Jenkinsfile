pipeline {
    agent none

    stages {
        stage('Hello') {
            agent { label 'robotfw' }
            steps {
                container('robotfw') {
                    echo 'Hello World'
                    echo 'Test auto build main'
                    sh 'python3 --version'
                    echo "Branch Triggered: ${BRANCH_NAME}"
                }
            }
        }
    }
}
