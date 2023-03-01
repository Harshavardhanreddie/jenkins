pipeline {
    agent none
    stages{
        stage('BUILD') {
            agent { label 'master' }
            steps{
                 sh '''
                    sleep 5
                    echo "This is a BUILD stage"
                 '''
            }
        }

        stage('TEST') {
            agent { label 'clabels' }
            steps{
                sh '''
                    sleep 6
                    echo "This is a TEST stage"
                '''
            }
        }

        stage('DEPLOY') {
            agent { label 'Jlabel' }
            steps{
                sh '''
                    sleep 5
                    echo "This is a DEPLOY stage"
                    
                '''
            }
        }
    }
}



