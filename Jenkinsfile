pipeline{
    agent any
    stages{
        stage('First'){
            steps{
                environment { 
                    EXECUTE='True'
                } 
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
