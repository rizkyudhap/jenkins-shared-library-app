pipeline {
	agent {
	 node {
	  label "linux && java11"
         }
        } 
	stages {
		stage ("Build") {
			steps {
				echo "Ini adalah Build Stage 1"
				echo "Ini adalah Build Stage 2"
				echo "Ini adalah Build Stage 3"
				sleep(2)
			}
		}
		stage ("Test") {
			steps {
				echo "Ini adalah Test Stage 1"
				echo "Ini adalah Test Stage 2"
				echo "Ini adalah Test Stage 3"
				sleep(2)
			}
		}
		stage ("Deploy") {
			steps {
				echo "Ini adalah Deploy Stage 1"
				echo "Ini adalah Deploy Stage 2"
				echo "Ini adalah Deploy Stage 3"
				sleep(2)
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