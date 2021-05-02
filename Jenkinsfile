pipeline {
agent any 

environemnt{

    IPaddress = hostname -I
}


stages{

  stage('inital')
{
  script{
   switch(env.Server){
   case 'Test':
                    env.Test1= "IP addresse"
                    break;
    case 'Test':
                    env.Test2= "IP addresse"
                    break;
   }
  }  
}  
    
 stage('git') {
     steps   {

         sh ' git clone  https://github.com/devops-34/16april'
     }
 }
 
 
}

stage ('two')
when {
				environment name: 'Test1', value: 'Test'
			}

 steps   {

         sh 'IPaddress'
     }
}
