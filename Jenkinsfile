pipeline {
agent any
    stages{
        stage('build') {
            steps {
                echo "****Entering build block******"
                retry(3) {
                echo "Welcome to D4"
                error "Testing the retry block"
                }
                echo "After 3 times"
            }
        }
    }
}


