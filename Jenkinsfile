pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                sh 'echo Hello world from LDIA !'
            }
        }
        stage('Scan') {
            steps {
                sh '''
                sonar-scanner \
                -Dsonar.projectKey=Test_reactJS \
                -Dsonar.sources=. \
                -Dsonar.host.url=http://localhost:9000 \
                -Dsonar.token=sqp_278503846ca79508c24af84212d959a016bb1a9c
                '''
            }
        }
    }
}
