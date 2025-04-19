pipeline {
    agent {
        docker { image 'ubuntu'}
    }

    stages {
        stage('pulling git repo') {
            steps {
                script {
                    def sprint_no = "SP01"
                    currentBuild.displayName = "Release - ${sprint_no}"
                }
                git branch: 'main', url: 'https://github.com/bhsabishek/git_test'
                echo "We have got the git repo"
            }
        }
    }
}
