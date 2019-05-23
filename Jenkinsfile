pipeline {
    agent { dockerfile true }
    stages {
        stage('Build image') {
            app= docker.build("grv10/docker-react-cicd")
            echo "Build run"
        }
    }
}
