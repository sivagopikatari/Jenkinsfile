pipeline{
    agent any
    stages{
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
        stage("aghsv"){
        when{
        branch "lucky"
        }
            steps{
                echo "deploy to "
            }
        }
    }
}
