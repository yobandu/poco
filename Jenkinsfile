pipeline {
	agent any
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/jerry/apache-maven-3.9.5/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			
			sh 'cp target/poco.war /home/jerry/apache-tomcat-9.0.82/webapps'
			}}
			}}
		
