pipeline {
    agent any
    stages {
        stage('1-Build') {
            steps {
                echo "Start of Stage Build..."
            }
        }
        stage('2-Test') {
            steps {
                echo "Start of Stage Test..."
		        echo "-------test started-------"
                echo "Hello ${PROJECT_NAME}"
                echo "Owner is ${OWNER_NAME}"
                echo "End of Stage Build..."

                echo "-------test finished-------"
            }
        }
        stage('3-Deploy') {
            steps {
                echo "Start of Stage Deploy..."
                echo "Deploying......."
                echo "End of Stage Build..."
            }
        }
    }
}
