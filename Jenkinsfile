node {
   def mvnHome
   stage('Preparation') { // for display purposes


      // MultiBranch Pipeline/GitHub Organizationの場合
	 /checkout scm

      // Get the Maven tool.
      // ** NOTE: This 'M3' Maven tool must be configured
      // **       in the global configuration.
      mvnHome = tool 'M3'
   }
   stage('Build') {

	  sh "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore clean package"
   }
}