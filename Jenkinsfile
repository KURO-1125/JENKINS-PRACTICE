pipeline{
    agent any
    stages{
        stage("git-checkout"){
            steps{
                // Checking out the code from git
                git url : 'https://github.com/KURO-1125/JENKINS-PRACTICE.git', branch : 'main'
                
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