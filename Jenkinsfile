pipeline {
    agent any

    stages {
        stage('checkot ') {
            steps {
               checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/rajcocvs/git_practise6.git']])
            }
        }
        stage('build ') {
            steps {
              sh 'mvn clean package'
            }
        }
        
    }
}
