
pipeline {
   agent any
       stages {
             stage('build') {
                       steps {
                             sh 'sudo snap install flutter --classic'
                             //sh 'flutter pub add test_coverage'
                             }                               
                            }

             stage('test') {
                      steps {
                             //sh 'flutter test --coverage'
                              sh 'sonar-scanner \
  -Dsonar.projectKey=FLutter-test \
  -Dsonar.sources=. \
  -Dsonar.host.url=http://49.0.198.122:9000 \
  -Dsonar.login=3e464033edc7a99d84a7152b51da7b2c58c8781a'
                             }
                           }
            }
}
