@Library('multibranch-shared-library') _
pipeline {
    agent any
    stages {
        stage("monorepo-job") {
            steps {
                script {
                    multiPipelines()
                }
            }
        }
    }
}
