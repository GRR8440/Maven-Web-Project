#!groovy

node{
	stage('SCM checkout'){
		git 'https://github.com/GRR8440/Maven-Web-Project.git'
	}
	stage('compail-package'){
	// Get maven home path
		def MVN_home=tool name: 'MAVEN_HOME', type: 'maven'
		sh "{MAVEN_HOME}/bin/mvn package"
	}
		
}
	
