pipeline {
     agent any
    tools { nodejs "NodeJs" }
     stages {
        stage("Installation") {
            steps {
                sh "npm ci"
            }
        }
        stage("Test") {
            steps {
                sh "npm test"
            }
        }
        stage("Build") {
            steps {
                sh "npm run build"
            }
        }
        stage("Done") {
            steps {
                echo "Done with building and testing React APP"
            }
        }
    }
}
