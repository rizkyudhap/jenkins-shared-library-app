pipeline {
	agent {
	 node {
	  label "linux && java11"
         }
        } 
	stages {
		stage ("Build") {
			steps {
				echo "Ini adalah Build Stage"
			}
		}
		stage ("Test") {
			steps {
				echo "Ini adalah Test Stage"
			}
		}
		stage ("Deploy") {
			steps {
				echo "Ini adalah Deploy Stage"
			}
		}
	}
	post {
		always {
			echo "I Will Always Say Hello!"
		}
		success {
			echo "Alhamdulillah Sukses bro!"
		}
		failure {
			echo "Its Ok To Be Fail, We Try Again!"
		}
		cleanup {
			echo "Don't care if its's success or fail"
		}
	}
}