pipeline {
    agent any

    // stages {
    //     stage('Hello') {
    //         steps {
    //         git branch: 'main', credentialsId: 'git_hub', url: 'https://github.com/dheerendrabhandari8/jenkins-cicd-php-demo.git'  
    //         }
    //     }
   
     stage('deploy') {
            steps {
              sshagent(['ssh-agent']) {


                sh 'ssh -o StrictHostKeyChecking=no root@18.188.202.173' 
     sh ' scp -r /var/lib/jenkins/workspace/php_ssh/*  root@18.188.202.173:/var/www/html' 
              }
            }
   
    }
        
    }

