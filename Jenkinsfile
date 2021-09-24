pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '**']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/ajay5844/demo-merge.git']]])
            }
        }
        stage('message') {
            steps {
                echo "this is main branch job"
            }
        }
    }
}
