pipeline{
    agent {label: 'ubuntu'}
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
                // sh('''pwsh "hello.ps1"''') //Works fine.
                sh 'cd UnitTests'
                sh('''pwsh "DeduplicateUnitTest.ps1"''')
            }
        }
    }
}