pipeline {
    agent any

    stages {
        stage('checkout ') {
            steps {
               checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/githubkusumam/git_practise6.git']])
            }
        }
        stage('build ') {
            steps {
              sh 'mvn clean package'
            }
        }
        
    }
}
