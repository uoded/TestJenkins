pipeline {
    agent any
    stages {
        stage(' Clean') {
            steps {
                sh ' rm -r TestJenkins/'
            }
        }
        stage(' Clone') {
            steps {
                sh 'git clone https://github.com/uoded/TestJenkins.git'
            }
        }
        stage(' Run') {
            steps {
                sh 'cd TestJenkins && python3 jenkins.py'
            }
        }
    }

}
