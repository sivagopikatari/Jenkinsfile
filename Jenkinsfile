pipeline{
    agent any
    stages{
        stage("maven build"){
            when{
                branch "maven  lucky build"
            }
            steps{
                sh " clean package -DskipTests=true"
            }
        }
        stage("dev"){
        when{
        branch "develop"
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
