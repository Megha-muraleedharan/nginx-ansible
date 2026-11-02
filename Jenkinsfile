pipeline {
    agent any

    stages {
        stage('Deploy Nginx using Ansible') {
            steps {
                echo 'Starting Nginx deployment through Ansible'

                sh '''
                    ssh meghamurali@172.17.0.1 '
                        cd ~/nginx-ansible &&
                        git pull origin main
                    '
                '''
            }
        }
    }
}
