pipeline{
    agent{
        node{
            label "aws-slave"
            customWorkspace "/home/ec2-user/customWorkspace"
        }
    }
    environment {
        user_name="jeff"
    }
    stages{
        stage("Build Main"){
            when{
                 tag "2.0"
            }
            steps{
               echo "Deploying to production"
            }
        }
    }
}
