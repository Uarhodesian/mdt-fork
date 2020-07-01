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
		result=`you’ll be a Man, my son!`
		echo $result
		if ["$result"="1"]
		        then
			        echo "Test passed"
		        else
			        echo "Test failed"
			        exit 1
		        fi
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
