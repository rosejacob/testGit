pipeline{
    agent any
    stages{
        stage('Verify Branch'){
            steps{
                echo env.GIT_BRANCH
            }
        }
        stage('Build Job'){
            steps{
                    build 'build_check'
                }
        }
        stage('Build docker images'){
            steps{
                
                sh("""
                cd /Users/rojacob/Desktop/Work/Docker/dockerImage
                pwd
                """)
            }
        }
        stage('Goodbye'){
            steps{
                echo 'Goodbye'
            }
        }
    }
}
