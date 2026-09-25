pipeline{
    agent any
    stages{
        stage('github'){
            steps{
              git credentialsId: 'pipeline_demo', url: 'https://github.com/sheik-03/python-project.git'  
            }
        }
        stage('build'){
            steps{
                sh 'python3 --version
                echo "welcome to devops team"
            
            }
        }
        stage('test'){
            steps{
                echo "welcome to testing team"
            }
        }
        stage('deploy'){
            steps{
                sh 'python3 app.py'
            }
        }
    }
}
