pipeline{ 
 
  agent any

  tools{
    maven "mvn"
  }
  
  stages{
     
    stage('build'){
	sh "mvn compile"
     }
 
    stage("test"){
        sh "mvn clean test"
      }
~         

    stage("package"){
        sh "package -DskipTests"
     }          
