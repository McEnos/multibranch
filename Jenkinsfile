@Library('multibranch-shared-library') _
pipeline {
    agent any
    stages {
        stage("running monorepo-job") {
            steps {
                script {
                    multiPipelines()
                }
            }
        }
    }
}
