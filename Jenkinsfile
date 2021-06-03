String branchname = "master"
String repourl = "https://github.com/jeetp2001/ec2-docker-jenkins-repo1.git"

pipeline {
	agent any
	stages {
		stage ('one') {
			sh 'mkdir build'
			dir('build') {
				git branch: branchname, url: repourl
			}
			sh 'pwd'
			sh 'whoami'
		}
	}
}
