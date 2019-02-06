node{
	stage('SCM checkout'){
		git 'https://github.com/GRR8440/Maven-Web-Project.git'
	}
	stage('clean'){
	// Get maven home path
		def mvnHOME = tool name: 'M2_HOME', type: 'maven'
		sh "${mvnHOME}/bin/mvn clean"
	}
	stage('test'){
		def mvnHOME = tool name: 'M2_HOME', type: 'maven'
		sh "${mvnHOME}/bin/mvn test"
	}
	stage('install'){
		def mvnHOME = tool name: 'M2_HOME', type: 'maven'
		sh "${mvnHOME}/bin/mvn install"
	}
	stage('deploy'){
		def mvnHOME = tool name: 'M2_HOME', type: 'maven'
		sh "${mvnHOME}/bin/mvn deploy"
	
}
	
