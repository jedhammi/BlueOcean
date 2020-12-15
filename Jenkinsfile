pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        echo '..... Build Phase Started :: Compiling Source Code :: ......'
        sh 'cd java_web_code'
        sh 'pwd'
        sh 'mvn install'
        echo 'Maven build complete'
      }
    }
  }
}
