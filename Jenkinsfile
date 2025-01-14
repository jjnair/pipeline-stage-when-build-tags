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
                 buildingTag()
            }
            steps{
               echo "Deploying to production"
            }
        }
    }
}
