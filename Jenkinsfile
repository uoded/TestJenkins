node {

    stage(' Clone') {
        steps {
            git'https://github.com/uoded/TestJenkins.git'
        }
    }
    stage(' Run') {
        steps {
            sh 'cd TestJenkins && python3 jenkins.py'
        }
    }
}
