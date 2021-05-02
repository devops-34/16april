pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Deploy') {
            when {
                branch 'production'
                anyOf {
                    environment name: 'Test1', value: 'Test'
                    environment name: 'Test2', value: 'UAT'
                }
            }
            steps {
                echo 'Deploying'
            }
        }
    }
}
