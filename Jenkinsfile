pipeline {
    agent any
    stages{
        steps('Lint Check'){
            sh "echo Installing Jslint"
            sh "npm install jslint"
            sh "ls -ltr node_modules/jslint/bin"
            sh "~/node_modules/jslint/bin/jslint.js server.js"

        }
    }
}