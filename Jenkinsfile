pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: 'QA']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/ajay5844/demo-merge.git']]])
            }
        }
        stage('message') {
            steps {
                echo "this is QA branch job"
            }
        }
    }
}
