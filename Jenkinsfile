pipeline {
    agent any
    
    environment {
      
        DB_ENGINE = 'DB'
    }
    stages {
        stage('git') {
            steps {
                sh 'git clone https://github.com/devops-34/16april'
                
            }
        }
        stage{
        when {
				expression {
					return env.Server == 'Test1' || env.Server == 'Test2'
				}
        }
			}
        stage('Example Deploy') {
            when {
                branch 'Test1'
                  when 
                  allof { {
                    environment name: 'Test1', value: 'Test'
                    
                     
                }
            }
            steps {
                echo "Database engine is ${DB_ENGINE}"
                
                
            }
        }
    }
}
}
