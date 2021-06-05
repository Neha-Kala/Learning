pipeline {
    agent any

    stages {
        stage ('Verify Branch'){
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stage('Docker Build'){
            steps{
                cmd(script: 'docker images -a')
                cmd(script: """
                cd C/Users/Neha Kala/Desktop/Dockerfiles/DF/
                docker images -a
                docker build -t jenkins-pipeline .
                docker images -a
                cd ..
                """)
            }

        }
    }

    
    
}

