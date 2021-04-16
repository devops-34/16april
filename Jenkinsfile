pipeline {

       agent any
       stages{
         stage('one')
                steps { 
                    script {
                     switch (env.Pre) {
                         case 'Test1':
                         echo " this is Test1"
                         break;
                         case 'Test2':
                         echo "this is Test2"
                         break;
} 
                         
                     }
                 }
           stage('two')
           steps{

            script {
                switch(env.Post) {

                    case 'Test1':
                    echo "this is Test1"
                    break;
                    case 'Test2':
                    echo "this is Test2"
                    break;
                }

            }               
           }
       }
   }
