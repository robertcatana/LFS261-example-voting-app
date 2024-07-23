pipeline{
    agent any
    
    stages {
        stage("one"){
            steps{
                echo "step one"
				sleep 5
            }
        }
        stage("two"){
            steps{
                echo "step two"
				sleep 5
            }
        }
        stage("three"){
			when{
				branch 'master'
				changeset "**/worker/**"
			}
			steps{
				echo "step three"
				sleep 5
			}

        }
    }
    
    post{
        always{
            echo 'This pipeline is completed'
        }
    }
        
}

