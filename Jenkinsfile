pipeline{
	agent any
    stages{
      stage('Build Application'){
            steps {
              echo 'Application is building'
              bat 'mvn clean install'
            }
  
       }
       stage('Deploy Application'){
            steps {
              echo 'Application is deploying'
              bat 'mvn package deploy -DmuleDeploy'
            }
  
       }

}