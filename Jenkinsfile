pipeline{
	agent any
	
    stages{
      stage('Build'){
            steps {
              echo 'Application is building'
              bat 'mvn clean install'
            }
  
       }
       stage('Deploy'){
            steps {
              echo 'Application is deploying'
              bat 'mvn package deploy -DmuleDeploy'
            }
  
       }

}