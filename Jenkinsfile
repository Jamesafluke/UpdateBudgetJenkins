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
                sh "echo 'this is the unit tests stage'"
                sh pwd
                sh pwd
            }
        }

    }
}




// stage('checkout'){
//             steps {
//                 checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/jenkinsci/generic-webhook-trigger-plugin.git']])
//             }
//         }