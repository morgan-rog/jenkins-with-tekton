pipeline {
    agent any
    stages {
        stage('build'){
            steps {
                checkout scm
                tektonCreateRaw(input: "hello-world-run.yaml", inputType: "FILE", namespace: "tekton-pipelines")
            }
        }
    }
}