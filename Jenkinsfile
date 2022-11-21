pipeline{
        agent any
 
	stages{
            stage('Install Docker'){
                steps{
                    sh "curl https://get.docker.com | sudo bash"
                }
            }

	stages{
            stage('Install docker composer'){
                steps{
                    sh "sudo apt-get update
		sh sudo apt-get install docker-compose-plugin"
                }
            }
	stages{
            stage('Run App'){
                steps{
                    sh "sudo docker-compose up -d --build"
                }
            }
        }    
}
