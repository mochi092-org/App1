node {
   def mvnHome
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/mochi092-org/Test4.git'
      // Get the Maven tool.
      // ** NOTE: This 'M3' Maven tool must be configured
      // **       in the global configuration.
      mvnHome = tool 'M3'
   }
   stage('Build') {

      bat(/"${mvnHome}\bin\mvn" -Dmaven.test.failure.ignore clean package/)

   }
}