pipeline {
  agent any
  stages {
    stage('Git clone')
    {
      steps{
        git branch: 'main', url: 'https://github.com/Lavanya1112/python-flask-CICD.git'
      }
    }
    
    stage('Deploy') {
        steps {
            sh "nohup python3 app.py & "
        }
    }
}
}
