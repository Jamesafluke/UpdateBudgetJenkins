pipeline{
    agent any
    stages{
        stage("checkout"){
            steps{
                // checkout scm
                git branch: 'main', url: 'https://github.com/Jamesafluke/UpdateBudget2.git'
                // checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfig: [[url: 'https://github.com/jamesafluke/UpdateBudget2.git']])
            }
        }
        stage('unitTests'){
            steps{
                // sh('''test.sh''')
                pwsh "Get-Host" //Works fine.
                sh('''pwsh "hello.ps1"''')
            }
        }
    }
}