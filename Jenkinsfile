@Library('multibranch-shared-library') _

def changedSubmodule = script {
    return sh(script: 'git diff --name-only HEAD^..HEAD', returnStdout: true).trim().tokenize('/')[0]
}

if (changedSubmodule) {
    dynamicJobs(changedSubmodule)
} else {
    echo "No submodule changes detected. Skipping submodule builds."
}
