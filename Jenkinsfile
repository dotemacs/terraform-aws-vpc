node('terraform') {
  pipeline {
        stage('FMT') {
            steps {
                sh 'terraform fmt --check'
            }
        }
        stage('Validate') {
            steps {
                sh 'terraform init'
                sh 'terraform validate'
            }
        }
        // stage('Deploy') {
        //     steps {
        //         echo 'Deploying....'
        //     }
        // }
    }
}
