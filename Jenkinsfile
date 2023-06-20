pipeline {
		agent any
		
		stages {
			stage('Checkout'){
				steps {
					checkout SCM
					}}
			stage('Build') {
				steps {
					sh '/home/admin/DevOps_tools/apache-maven-3.9.2/bin/mvn install'
					}}
			stage('Deployment') {
				steps {
					sh 'cp artis.war /home/admin/DevOps_tools/apache-tomcat-9.0.76/webapps'
					}}}}
