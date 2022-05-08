pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.73   sudo apt update'
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.73   sudo apt -y install nomad'
                
            }

        }
        stage('SUPPRESSION') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.11   nomad'
               
            }

        }
       
    }
    
}
