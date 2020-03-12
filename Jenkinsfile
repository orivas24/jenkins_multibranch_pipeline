pipeline{
    agent any
    stages{
	environment{
		EXECUTE = true
	}
        stage('First'){
            steps{
                echo "Updating First Stage" 
            }
        }    
        stage('Second'){
            when {
                expression { EXECUTE == true }
            } 
            steps{
                echo "Updating Second Stage"
            }
        }
        stage('Third'){
             when {
                expression { EXECUTE == true }
            } 
            steps{
                echo "Updating Third Stage"
            }
        }
    }
}
