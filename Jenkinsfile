@Library("jenkins-shared-library@main") _

import rizkypratama.jenkins.Output;


pipeline {
    agent any
    stages {
        stage ("Hello Groovy") {
            steps {
                script {
                    Output.hello("Groovy")
                }
            }
        }
        stage ("Hello World") {
            steps {
                script {
                    hello.world()
                }
            }
        }
    }
}