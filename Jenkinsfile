String branchname = "master"
String repourl = "https://github.com/jeetp2001/ec2-docker-jenkins-repo1.git"

pipeline {
	agent any
	stages {
		stage ('one') {
			steps {
				git branch: branchname, url: repourl
				sh 'pwd'
				sh 'whoami'
				sh 'docker build -t apacheimg ./build/apache/'
				sh 'docker run -d -p 80:80 --name apachecon apacheimg'
			}
		}
	}
}
