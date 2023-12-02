@Library("multibranch-shared-lib") _
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
