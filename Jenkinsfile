pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        // Checkout the Git repository
        git 'https://github.com/Udaychinnala/hello-world-war.git'
      }
    }
    stages {
        stage('Git Tagging') {
            steps {
                script {
                    def tagName = "UDAY" // Set your desired tag name here
                    sh "git tag ${tagName}" // Creates the Git tag
                    sh "git push origin ${tagName}" // Pushes the tag to the remote repository
                }
            }
        }
        // Other stages in your pipeline...
    }
}
