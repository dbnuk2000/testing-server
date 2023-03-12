pipeline {
    agent none

    stages {

        stage ('The beginning') {
            agent any

            steps {
                echo 'Hello, '

                sh '''#!/bin/bash

                    apt update -yq
                    echo "Updating System"
                '''
            }
        }
        stage ('The next stage') {
            agent any
            
            steps {
                echo 'The next stage'
                
                sh '''#!/bin/bash
                
                    apt upgrade -yq
                    echo "Upgrading System"
                '''    
            }
        }
    }
}
