pipeline {
    agent none
    environment {
          HAR = "1"
    }
    stages{
        stage('BUILD') {
            agent { label 'master' }
            steps{
                 sh '''
                    sleep 5
                    echo "This is a BUILD stage and $HAR"
                 '''
            }
        }

        stage('TEST') {
            agent { label 'clabels' }
            steps{
                sh '''
                    sleep 6
                    echo "This is a TEST stage and $HAR"
                '''
            }
        }

        stage('DEPLOY') {
            agent { label 'Jlabel' }
            steps{
                sh '''
                    sleep 5
                    echo "This is a DEPLOY stage and $HAR"
                    
                '''
            }
        }
    }
}


