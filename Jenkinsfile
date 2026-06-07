pipeline {
    agent any

    triggers {
        // Activates the webhook listener for Smee.io/GitHub
        githubPush() 
    }

    stages {
        stage('Pull and Check Code') {
            steps {
                echo '=== Success! Git code has been downloaded to Jenkins ==='
                
                // This command lists your repository files inside your RHEL 9 container
                sh 'ls -la'
            }
        }
    }
}
