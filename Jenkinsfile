node{
	stage('SCM checkout'){
		git 'https://github.com/GRR8440/Maven-Web-Project.git'
	}
	stage('clean'){
	// Get maven home path
		def mvn_HOME = tool name: 'mvn_HOME', type: 'maven'
		sh "${mvn_HOME}/bin/mvn clean"
	}
	stage('test'){
		def mvn_HOME = tool name: 'mvn_HOME', type: 'maven'
		sh "${mvn_HOME}/bin/mvn test"
	}
	stage('install'){
		def mvn_HOME = tool name: 'mvn_HOME', type: 'maven'
		sh "${mvn_HOME}/bin/mvn install"
	}
	stage('deploy'){
		def mvn_HOME = tool name: 'mvn_HOME', type: 'maven'
		sh "${mvn_HOME}/bin/mvn deploy"
	}
}
	
