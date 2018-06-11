node {
   
   stage('Code Checkout') { // for display purposes
     git credentialsId: 'GithubID', url: 'https://github.com/IndianTeamA/ui_project.git'
   }
   stage('Build') {
    sh 'mvn clean compile'  
   }
   stage('Test') {
    sh 'mvn test'
   }
   stage('Archive Artifactory') {
     sh 'mvn install'
   }
   
   stage('Deploy to Dev') {
    
   }
}
