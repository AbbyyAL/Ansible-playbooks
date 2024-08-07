pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/AbbyyAL/Ansible-playbooks.git', branch: 'main'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                sh './configure_router.sh'
            }
        }
    }
}
