pipeline {
    agent any

    stages {
        // stage('Hello') {
        //     steps {
        //     git branch: 'main', credentialsId: 'git_hub', url: 'https://github.com/dheerendrabhandari8/jenkins-cicd-php-demo.git'  
        //     }
        // }
  //  stage('deploy') {
  //          steps {
  // sh "echo from main branch"
  
  //          }
     stage('deploy') {
            steps {
              sshagent(['ssh-agent']) {


                //   sh 'ssh -o StrictHostKeyChecking=no ubuntu@18.216.230.49' 
     sh ' scp -r /var/lib/jenkins/workspace/new_multi_main/*  root@18.188.202.173:/var/www/html' 
              }
            }
   
    }
        
    }
}

