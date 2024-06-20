pipeline {
    agent any
     parameters {
        string(name: 'p_developer', defaultValue: 'GGman', description: 'Developer to greet')
        string(name: 'p_greets', defaultValue: 'Hello World', description: 'Greeting message')
    }
    triggers {
        cron('H */2 * * *')
    }
    stages {
        stage('Build') {
            steps {
                bat 'C:/Jenkins/test.bat' 
            }
        }
        stage('Test') {
            steps {
                bat 'C:/Jenkins/test.bat'
            }
        }
        stage('Package') {
            steps {
                bat 'C:/Jenkins/test.bat'
            }
        }
        stage('Deploy') {
            steps {
                bat 'C:/Jenkins/test.bat'
            }
        }
        stage('Greet') {
            steps {
                script {
                    echo "${params.p_greets}, ${params.p_developer}!"
                }
            }
        }
    }
}
