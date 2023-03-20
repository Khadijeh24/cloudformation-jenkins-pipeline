pipeline {
agent any 
  stages {
    stage('Clone Repo') {
      steps {
        sh "export AWS_DEFAULT_REGION=us-east-1"
        sh "aws cloudformation create-stack --stack-name laxmiEc2InstanceStack --template-body file://laxmi-ec2.yaml --region 'us-east-1'"
      }
    }
  }

}
