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
                
                sh(script: """
                cd /Users/rojacob/Desktop/Work/Docker/dockerImage
                docker build -t dockeer-pipeline .
                docker ps -a
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
