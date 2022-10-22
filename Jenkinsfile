pipeline{
    agent any
    stages{
        stage("lucky"){
        when{
        branch "lucky"
        }
            steps{
                sh " clean package -DskipTests=true"
            }
        }
        stage("dev"){
        when{
        branch "dev"
        }
            steps{
                echo "deploy to dev"
            }
        }
                stage("stage"){
                when {
                branch "stage"
                }
            steps{
                echo "deploy to stage"
            }
        }
                        stage("main"){
                        when {
                        branch "main"
                        }
            steps{
                echo "deploy to main"
            }
        }
    }
}
