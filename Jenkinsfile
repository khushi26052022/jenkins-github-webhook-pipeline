pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Pull Code from Develop Branch') {
            steps {
                sh '''
                mkdir -p /home/ubuntu/git-code
                cd /home/ubuntu/git-code
                rm -rf *
                git clone -b develop https://github.com/khushi26052022/jenkins-git-pipeline.git .
                '''
            }
        }
    }
}
