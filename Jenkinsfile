pipeline {
    agent any

    environment {
        PROJECT_NAME = 'MyApp'
        DEPLOY_ENV = 'dev'
    }

    stages {

        stage('Init') {
            steps {
                echo "🔧 Initializing pipeline for ${PROJECT_NAME}"
            }
        }

        stage('Build') {
            when {
                environment name: 'DEPLOY_ENV', value: 'dev'
            }
            steps {
                echo "🛠️ Building project for ${DEPLOY_ENV} environment"
                sh 'ls -al'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                sh 'echo Simulating tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying the app...'
                sh 'echo App deployed!'
                echo 'I am MohamedMabroukMohamedRashad'
            }
        }
    }
}

