pipeline
  {
  agent any
   stages{
    stage('Build Application'){
     steps{
      bat 'mvn clean install'
        }
      }
      
    stage('Deploy Application to Cloudhub'){
     steps{
      bat 'mvn package deploy -Dusername=prameelak -Dpassword=Padcha@04 -Denvironment=Sandbox -Dmule.version=4.3.0 -Dworkers=1 -Dworker.type=MICRO -Dapplication.name=soaptorest-sys-api-v1 -DmuleDeploy'
      }      
     }  
   }
} 