pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'sh \'pandock -s /home/kader/index.md  -o index.html\''
        sh 'sh \'pandock -s /home/kader/index.md  -o index.docx\''
      }
    }

    stage('Deploy') {
      steps {
        sh 'sh \'mv index.html /var/html\''
        sh 'sh \'mv index.html /var/html/doc\''
      }
    }

  }
}