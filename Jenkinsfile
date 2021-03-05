node (label: 'JenkinsNode1-Maven-Ubuntu') {

   stage('SCM') {
      // git clone
	  git 'https://github.com/devopstasks/SpringPetClinic.git'
   }
   
   stage ('build the packages') {
      // mvn package
	  sh 'mvn package'
   }

   
   
   stage ('archival') {
     // archiving artifacts
	 archive 'target/*.jar'
   }

}
