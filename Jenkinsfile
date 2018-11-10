node{
	stage('SCM checkout'){
		git 
	}
	stage('compail-package'){
	// Get maven home path
		def mvnHOME = tool name: 'MAVEN_HOME', type: 'maven'
		sh "${mvnHOME}/bin/mvn package"
	}
		
}
	
