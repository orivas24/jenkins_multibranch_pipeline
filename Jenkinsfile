pipeline{
    agent any
    stages{
        stage('First'){
            environment { 
                    EXECUTE='True'
                }
            steps{
                echo "Updating First Stage" 
            }
        }    
        stage('Second'){
            when {
                expression { EXECUTE == 'True') }
            } 
            steps{
                echo "Updating Second Stage"
            }
        }
        stage('Third'){
             when {
                expression { EXECUTE == 'True') }
            } 
            steps{
                echo "Updating Third Stage"
            }
        }
    }
}
