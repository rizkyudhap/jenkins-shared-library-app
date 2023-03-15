pipeline {
	agent {
	 node {
	  label "linux && java11"
         }
        } 
	stages {
		stage ("Build") {
			steps {
				script {
					for (int i = 0; i<10; i++) {
						echo("Script ${i}")
					}
				}
				echo "Start Build"
				echo "Finish Build"
			}
		}
		stage ("Test") {
			steps {
				script {
					def data [
						"firstName = Rizky"
						"lastName = Pratama"
					]
					writeJSON(file: "data.json", json: data)
				}
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