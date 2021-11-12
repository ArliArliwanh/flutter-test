
pipeline {
agent any
stages {
stage('build') {
steps {
sh 'cd project/'

sh 'sudo snap install flutter --classic'
sh 'ls'

sh 'cd project | flutter pub add test_coverage'
}
}

stage('test') {
steps {
sh 'flutter test --coverage'
}
}

}
