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
                sh "whoami"
                sh "pwd"
                pwsh "Get-Host"
                // powershell "Write-Host 'Testing powershell'"
            }
        }
    }
}




// stage('checkout'){
//             steps {
//                 checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/jenkinsci/generic-webhook-trigger-plugin.git']])
//             }
//         }