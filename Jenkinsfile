pipeline {
    agent { 
        node {
            label 'my_pc'
            }
      }
    triggers {
        pollSCM '* * * * *'
    }
     stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''#!/bin/bash
                echo "doing Building.."
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''#!/bin/bash
                echo "doing Testing.."
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo "doing delivery stuff.."
            }
        }
    }
}
