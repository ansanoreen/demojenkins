pipeline {
    agent any

    stages {
         stage('timestamp')
        {
            steps {
                sh 'date'
                sh 'pwd'
            }
        }
        stage('build')
        {
            steps {
                echo 'build app'
            }
        }
        stage('test')
        {
            steps {
                echo 'test app'
            }
        }
        stage('deploy')
        {
            steps {
                echo 'deploy app'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'summery', subject: 'pipeline status', to: 'adeelansa006@gmail.com'
        }
    }
    }

