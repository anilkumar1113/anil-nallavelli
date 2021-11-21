pipeline {
    agent any

    stages {
        stage('scm stage') {
            steps {
                echo 'Hello batch7 devops champs'
                git 'https://github.com/wakaleo/game-of-life.git'
            }
        }
    }
    stage('deploy to tomcat stage') {
            steps {
                echo 'deploy to srinu tomcat'
                deploy adapters: [tomcat9(credentialsId: '02b632eb-df64-4af3-bf54-a5cb2684353f', path: '', url: 'http://107.21.193.86:8080/')], contextPath: 'batch7', war: '**/*.war'
            }
        }
}
 
 
