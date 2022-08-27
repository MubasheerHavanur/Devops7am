pipeline {
    agent any
    stages{
        stage('build_app') {
            steps {
                sh 'echo "this is first build running on 'hostname' host"'
            }
        }
        stage('app_testing') {
            steps {
                sh 'echo "this is second build running on 'hostname' host"'
            }
        }
    }
}
