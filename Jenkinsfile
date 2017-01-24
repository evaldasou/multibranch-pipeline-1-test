node {
   stage('Git') {
      git 'https://github.com/evaldasou/multibranch-pipeline-1-test.git'
   }
   stage('Build') {
       def builds = [:]
       builds['scala'] = {
           echo 'building the scala'
       }
       builds['frontend'] = {
           echo 'building the frontend'
       }
     parallel builds
   }
   stage('Results') {
        echo 'results'
   }
}
