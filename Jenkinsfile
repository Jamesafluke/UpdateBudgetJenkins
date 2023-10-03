pipeline{
    agent {label 'ubuntu'}
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
                dir('UnitTests/DeduplicateUnitTest'){
                    sh('''pwsh "DeduplicateUnitTest.ps1"''')
                }
                dir('UnitTests/ArbitraryExceptionsUnitTest'){
                    sh('''pwsh "ArbitraryExceptionsUnitTest.ps1"''')
                }
                dir('UnitTests/DetermineMethodUnitTest'){
                    sh('''pwsh "DetermineMethodUnitTest.ps1"''')
                }
            }
        }
    }
}