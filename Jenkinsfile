pipeline {
    agent { 
        docker { 
            image 'maven:3.3.3' 
        } 
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('Sanity check') {
            input "Does the build look okay?"   
        }
        stage('Deploy to production') {
            echo 'Deploying'
        }
    }
}
