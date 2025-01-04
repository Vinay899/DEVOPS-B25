pipeline 
{
	agent any
	tools
	{
		maven 'MAVEN_HOME'
	}
	
	stages{
		stage('Welcome Master Branch')

		{
			steps
			{
				echo 'Welcome to Jenkins Pipeline'
			}			
		}
		stage('Checkout') 
		{
        		steps 
			{                
           			 git 'https://github.com/hkshitesh/DEVOPS-B25.git'
        		}
		}
		stage('Clean Stage')
		{
			steps
			{
				sh 'mvn clean'
			}			
		}
		stage('Test Stage')
		{
			steps
			{
				sh 'mvn test'
			}			
		}
		stage('Build Stage')
		{
			steps
			{
				sh 'mvn install'
			}			
		}
		stage('Java Version Check Stage')
		{
			steps
			{
				sh 'java --version'
			}			
		}
		
		stage('Success Stage')
		{
			steps
			{
				echo 'Successfully Build Thanks'
			}			
		}
	
	}
}
