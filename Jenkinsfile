pipeline {
    agent any
    
    environment {
      
        DB_ENGINE    = 'DB'
    }
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Deploy') {
            when {
                branch 'Test1'
                  allOf {
                    environment name: 'Test1', value: 'Test'
                    environment name: 'UAT', value: 'Test'
                     
                }
            }
            steps {
                echo "Database engine is ${DB_ENGINE}"
                
                
            }
        }
    }
}
