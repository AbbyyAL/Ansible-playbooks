pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/AbbyyAL/Ansible-playbooks.git', branch: 'main'
            }
        }
        stage('Set Permissions') {
            steps {
                sh 'chmod +x ./configure_router.sh'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                sh './configure_router.sh'
            }
        }
    }
}
