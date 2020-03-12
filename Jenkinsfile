pipeline{
    agent any
    stages{
        stages('First'){
            environment { 
                    EXECUTE='True'
                }
            steps{
                echo "Updating First Stage" 
            }
        }    
        stage('Second'){
            when {
                environment name: 'EXECUTE', value: 'TRUE'
            } 
            steps{
                echo "Updating Second Stage"
            }
        }
        stage('Third'){
             when {
                environment name: 'EXECUTE', value: 'TRUE'
            } 
            steps{
                echo "Updating Third Stage"
            }
        }
    }
}
