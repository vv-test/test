pipeline {
	agent any
	
	stages {
		stage ('_____Compile stage') {
			steps {
				withMaven(maven : 'maven_360') {
					sh 'mvn clean compile'
				}
			}
		}
		
		stage ('_____Test stage') {
			steps {
				withMaven(maven : 'maven_360') {
					sh 'mvn clean test'
				}
			}
		}
		
		stage ('_____Deploy stage') {
			steps {
				withMaven(maven : 'maven_360') {
					sh 'mvn clean deploy'
				}
			}
		}
		
	}
}