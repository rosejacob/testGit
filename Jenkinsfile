pipeline{
    agent any
    stages{
        stage('Verify Branch'){
            steps{
                echo $GIT_BRANCH
            }
        }
        stage('Build Job'){
            steps{
                    build 'build_check'
                }
    
        stage('Goodbye'){
            steps{
                echo 'Goodbye'
            }
        }
    }
}
