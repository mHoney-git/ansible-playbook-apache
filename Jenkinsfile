pipeline {
    agent any 
    stages {
        stage ('installing apache on apache-web server') {
            steps {
                ansiblePlaybook credentialsId: 'AWS-SSH-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'hosts.inv', playbook: 'apache.yml'
              }
        }
    }
}