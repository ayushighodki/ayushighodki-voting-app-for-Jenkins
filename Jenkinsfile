pipeline {
   agent any

   stages {
      stage('Verify Branch') {
         steps {
            echo "$GIT_BRANCH"
         }
      }
   stage('build') {
         steps {
            powershell 'Write-output "Build Successfull from jenkinsfile!"'
       }
   }
   }
}
