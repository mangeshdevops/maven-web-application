node {
	echo "GitHub BranhName ${env.BRANCH_NAME}"
	echo "Jenkins Job Number ${env.BUILD_NUMBER}"
	echo "Jenkins Node Name ${env.NODE_NAME}"
	echo "Jenkins Home ${env.JENKINS_HOME}"
	echo "Jenkins URL ${env.JENKINS_URL}"
	echo "JOB Name ${env.JOB_NAME}"
	
	stage("CheckOutCodeGit") {
		git branch: 'master', url: 'https://github.com/mangeshdevops/maven-web-application.git'
	}
	
	stage("Build") {
		sh "mvn clean package"
	}
}	 
