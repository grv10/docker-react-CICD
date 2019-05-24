pipeline {
    agent { 
            dockerfile {
            filename 'Dockerfile.dev'
            label 'grv10/docker-react-cicd'
            }
        }
    stages {
            stage('Before install, Build image') {
            app= docker.build("grv10/docker-react-cicd")
            echo "Build run"
        }
        
        stage('Run test script'){
            
        }
        
        stage('Deploy to EB'){
            environment{
                AWS_CREDS= credentials('predefined credentials')   
            }
        }        
    }
}
