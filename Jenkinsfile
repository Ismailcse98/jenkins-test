pipeline {
    agent any

    parameters {
        choice(name: 'ENVIRONMENT', choices: ['dev', 'staging', 'prod'], description: 'Select the environment to deploy')
    }

    stages {
        stage('Print Selected Environment') {
            steps {
                echo "Selected Environment: ${params.ENVIRONMENT}"
            }
        }

        stage('Conditional Execution') {
            steps {
                echo "Deploying to Development environment"
            }
        }
    }
}
