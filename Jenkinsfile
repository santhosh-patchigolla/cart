// NodeJs

pipeline {
    agent { label 'work-station' }
    stages {
        stage ('Lint Check') {                      // start the stage
            steps {
                sh "echo installing JSlint"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js || true"   // this double pipe symbol includes that if the first command is failure make it as a true statement
            }
        }
        stage('Code Compile') {
            steps {
                sh "npm install"
            }
        }                                               // end of this stage
    }
}


