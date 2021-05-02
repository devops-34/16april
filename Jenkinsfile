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
     steps 
 }
 sh ' git clone
 
}

stage ('two')
when {
				environment name: 'Test1', value: 'Test'
			}


}
