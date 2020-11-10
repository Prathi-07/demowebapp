node
   stages {
      stage('GIT') {
         steps {
            // Get some code from a GitHub repository
            git 'https://github.com/Prathi-07/demowebapp.git'
         }
      }
      stage('Build') {
         steps {
            def mvnhome= tool name: 'MAVEN_HOME', type: 'maven'
            sh "${mvnhome}/bin/mvn clean package"
         }
      }
   }

