pipeline {
    agent { label 'Jlabel' } 
    parameters {
         string defaultValue: 'main', name: 'Branch', trim: true
     }
    
    environment {
        BRANCH_NAME = "${Branch}"
    }
    stages{
        stage('BUILD') {
            
            steps{
                 sh '''
                    sleep 5
                    echo "This is a BUILD stage and $HAR"
                 '''
            }
        }

        stage('TEST') {
            
            steps{
                sh '''
                    sleep 6
                    echo "This is a TEST stage and $HAR"
                '''
            }
        }

        stage('DEPLOY') {
            
            steps{
                sh '''
                    sleep 5
                    echo "This is a DEPLOY stage and $HAR"
                    
                '''
            }
        }
    }
}


