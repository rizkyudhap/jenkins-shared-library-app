pipeline {
	agent {
	 node {
	  label 'linux && java11'
         }
        } 
	stages {
		stage ('Hello') {
			steps {
				echo ('Hello Rizky Pratama!')
			}
		}
	}
}
	post {
		always {
			echo 'I Will Always Say Hello!'
		}
		success {
			echo 'Alhamdulillah Sukses bro!'
		}
		failure {
			echo 'Its Ok To Be Fail, We Try Again!'
		}
		cleanup {
			echo "Don't care if its's success or fail"
		}
	}