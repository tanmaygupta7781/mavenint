pipeline{
	agent any
	
	tools{
	 maven 'Maven'
	 }
	
	stages{
	 stage('checkout')
	 {
	  steps
	  {
	    git branch:'master', url:'https://github.com/tanmaygupta7781/mavenint.git'
	   }
	  }
	  stage('compile')
	  {
	   steps{
	    sh 'mvn compile'
	    }
	   }
	  stage('test')
	  {
	   steps{
	    sh 'mvn test'
	    }
	   }
	  stage('package')
	  {
	  	steps{
	  	 sh 'mvn package'
	  	 }
	  	}
	  }
	}
