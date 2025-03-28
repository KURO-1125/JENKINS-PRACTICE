pipeline{
    agent any
    stages{
        stage("git-checkout"){
            steps{
                echo "Checking out the code from git"
            }
        }
        stage("BUILD"){
            steps{
                echo "BUILDING KURO"
            }
        }
        stage("TEST"){
            steps{
                echo "TESTING KURO"
            }
        }
        stage("DEPLOY"){
            steps{
                echo "DEPLOYING KURO"
            }
        }
    }
}