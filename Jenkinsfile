
pipeline {
   agent any
       stages {
             stage('build') {
                       steps {
                             sh 'sudo snap install flutter --classic'
                             sh 'flutter pub add test_coverage'
                             }                               
                            }

             stage('test') {
                      steps {
                             sh 'flutter test --coverage'
                             }
                           }
            }
}
