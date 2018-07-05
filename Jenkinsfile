node {
   stage('Preparation') {
      git 'https://github.com/sreeket/ReleaseAndDeployment.git'
   }
   stage('Build') {
      sh "./gradlew clean test"
   }
   stage('Deploy') {
      sh "git push https://git.heroku.com/boiling-castle-45041.git master"
   }
}