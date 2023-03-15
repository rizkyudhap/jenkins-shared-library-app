pipeline {
	agent {
	 node {
	  label "linux && java11"
         }
        } 
	stages {
		stage ("Build") {
			steps {
				echo "Start Build"
				sh("./mvnw clean compile test-compile")
				echo "Finish Build"
			}
		}
		stage ("Test") {
			steps {
				echo "Start Test"
				sh("./mvnw test")
				echo "Finish Test"
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