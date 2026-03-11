pipeline {
    agent any

    environment {
        AWS_DEFAULT_REGION = 'ap-south-1'
        S3_BUCKET = 'amz-s3-0111'
    }

    stages {

        stage('Delete Old Files From S3') {
            steps {
                sh 'aws s3 rm s3://$S3_BUCKET --recursive'
            }
        }

    }
}
