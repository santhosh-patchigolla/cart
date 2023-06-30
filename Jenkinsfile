// NodeJs

pipeline {
    agent { label 'work-station' }
    stage {
        stages('Lint Check') {                      // start the stage
            steps {
                sh "echo installing JSlint"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js"
            }
        }                                                       // end of this stage
    }
}


