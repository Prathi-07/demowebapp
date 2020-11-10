node{
  stage('GIT') {
    git 'https://github.com/Prathi-07/demowebapp.git'
  }
   stage('Build') {
     def mvnhome= tool name: 'MAVEN_HOME', type: 'maven'
       sh "${mvnhome}/bin/mvn clean package"
   }
}

