pipeline {
	agent any
		
	stages {
		stage ("pull scm") {
			steps {
				git pull url: 'https://github.com/himanshu27797/python-pipeline.git'
				}
			}
		stage ("Build") {
			steps {
				sh 'python3 -V'
				sh 'python3 cp.py'
				}
			}
		stage ("Test") {
			steps {
				sh 'python3 test.py'
				}
			}
		}
	}
