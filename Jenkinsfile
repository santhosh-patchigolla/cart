// NodeJs

pipeline {
    agent { label 'work-station' }
    stages {
        stage ('Lint Check') {                      // start the stage
            steps {
                sh "echo installing JSlint"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js"
            }
        }
        stage('Code Compile') {
            steps {
                sh "npm install"
            }
        }                                               // end of this stage
    }
}


