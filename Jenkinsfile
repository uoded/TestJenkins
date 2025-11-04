pipeline {
    agent any
    stages {
        stage(' Clean') {
            steps {
                sh ' rm -rf TestJenkins/'
            }
        }
        stage(' Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/uoded/TestJenkins.git'
                // sh 'git clone https://github.com/uoded/TestJenkins.git'
            }
        }
        stage(' Run') {
            steps {
                sh 'cd TestJenkins && python3 jenkins.py'
            }
        }
    }

}
