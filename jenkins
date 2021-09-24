pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: 'dev']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/ajay5844/demo-merge.git']]])
            }
        }
        stage('message') {
            steps {
                echo "this is Dev branch job"
            }
        }
    }
}
