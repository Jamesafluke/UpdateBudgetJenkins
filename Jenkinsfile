pipeline{
    agent any
    stages{
        stage("checkout"){
            steps{
                checkout scm
                // checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfig: [[url: 'https://github.com/jamesafluke/UpdateBudget2.git']])
            
            }
        }
        stage('unitTests'){
            steps{
                sh hello.sh
            }
        }

    }
}




// stage('checkout'){
//             steps {
//                 checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/jenkinsci/generic-webhook-trigger-plugin.git']])
//             }
//         }