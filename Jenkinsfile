pipeline {
    agent any
    environment {
      PROJECT_NAME = "Pipeline"
      OWNER_NAME   = "Oleksii Danyliuk"
    }

    stages {
        stage('1-Build') {
            steps {
                echo "Start of Stage Build..."
		cat index.html
            }
        }
        stage('2-Test') {
            steps {
                echo "Start of Stage Test..."
		echo "-------test started-------"
                echo "Hello ${PROJECT_NAME}"
                echo "Owner is ${OWNER_NAME}"

		echo "-------test finished-------"
            }
        }
    }
}
