pipeline{
    agent any
    tools{
        maven 'Maven'
    }
    stages{
        stage("Build"){
            steps{
                sh 'mvn clean package'
            }
        }
        stage("Test"){
            steps{
                sh 'mvn test'
            }
        }
        stage("Run JAR"){
            steps{
                scripts{
                    // Run the JAR file and capture the output
                    def output = sh(script:'java -jar target/simple-java-project-1.0-SNAPSHOT.jar', returnStdout:true).trim()

                    // Print the output to jenkins console
                    echo "Output from JAR : ${output}"
                }
            }
        }
    }
}