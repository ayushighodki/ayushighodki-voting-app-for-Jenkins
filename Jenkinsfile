pipeline {
   agent any

   stages {
      stage('Verify Branch') {
         steps {
            echo "$GIT_BRANCH"
         }
      }
   }
   stages {
      stage('Docker build') {
         steps {
            pwsh(script:'docker images -a')
			pwsh(script:"""
			cd azure-vote/
			docker images -a
			docker build -t jenkins-pipeline.
			cd..
			""")
         }
      }
   }
}
