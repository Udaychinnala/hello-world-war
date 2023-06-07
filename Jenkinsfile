pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        // Checkout the Git repository
        git 'https://github.com/Udaychinnala/hello-world-war.git'
      }
    }
    stage('Create Git Tag') {
      steps {
        script {
          def tag = "uday" // Specify the tag name you want to create
          // Create the Git tag
          sh "git tag ${tag}"
          // Push the Git tag to the remote repository
          sh "git push origin ${tag}"
        }
      }
    }
  }
}
