pipeline{
    agent any
    stages{
        stages('ONE'){
            steps{
                sh '
                echo "Step One"
                ' 
            }
        }    
        stage('Two'){
            steps{
                sh '
                echo "Step Two"
                '
            }
        }
        stage('Three'){
            steps{
                sh '
                echo "Step Three"
                '
            }
        }
    }
}
