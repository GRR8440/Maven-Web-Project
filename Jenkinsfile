node{
	stage('SCM checkout'){
		git 'https://github.com/GRR8440/Maven-Web-Project.git'
	}
	stage('clean'){
	// Get maven home path
		def mvnHOME = tool name: 'MAVEN_HOME', type: 'maven'
		sh "${mvnHOME}/bin/mvn clean"
	}
	stage('test'){
		sh "${mvnHOME}/bin/mvn test"
	}
	stage('install'){
		sh "${mvnHOME}/bin/mvn install"
	}
	stage('deploy'){
		sh "${mvnHOME}/bin/mvn deploy"
	}
		
}
	
