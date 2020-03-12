pipeline{
    agent any
    stages{
        stage('First'){
            environment { 
                    EXECUTE = 'True'
                }
            steps{
                echo "Updating First Stage" 
            }
        }    
        stage('Second'){
            when {
                environment name: 'EXECUTE', value: 'True'
            } 
            steps{
                echo "Updating Second Stage"
            }
        }
        stage('Third'){
             when {
                environment name: 'EXECUTE', value: 'True'
            } 
            steps{
                echo "Updating Third Stage"
            }
        }
    }
}
