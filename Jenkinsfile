pipeline{
    agent any
    
    stages {
        stage("one"){
            steps{
                echo "step one"
            }
        }
        stage("two"){
            steps{
                echo "step two"
            }
        }
        stage("three"){
            steps{
                echo "step three"
            }
        }
    }
    
    post{
        always{
            echo 'This pipeline is completed'
        }
    }
        
}
