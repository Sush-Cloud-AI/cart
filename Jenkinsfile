pipeline {
    agent any
    stages{
        stage('Lint Check'){
            steps{
            sh "echo Installing Jslint"
            sh "npm install jslint"
            sh "ls -ltr node_modules/jslint/bin"
            sh "~/node_modules/jslint/bin/jslint.js server.js"

        }
    }
}

}