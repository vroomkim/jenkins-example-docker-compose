pipeline {
    agent any
    stages {
        state("verify tooling") {
            steps {
                sh '''
                  docker version
                  docker info
                  docker compose version
                  curl --version
                  jq --version
                '''
            }
        }
    }
}