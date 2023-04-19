pipeline {
    agent any
    stages{
        // should run on every coomit to feautre branch 
        stage('Lint Check'){
            steps{
            sh "echo Installing Jslint"
            sh "npm install jslint"
            sh "ls -ltr node_modules/jslint/bin"
            sh "~/node_modules/jslint/bin/jslint.js server.js" || true   // true is used to mark the present step as pass and skip to next step  even if lint check fails  

        }
    }
}

}