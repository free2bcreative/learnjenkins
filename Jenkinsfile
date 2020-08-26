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
            steps {
                input "Does the build look okay?"   
            }
        }
        stage('Deploy to production') {
            steps {
                echo 'Deploying'
            }
        }
    }
}
