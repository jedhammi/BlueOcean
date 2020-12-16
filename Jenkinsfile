pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        echo '..... Build Phase Started :: Compiling Source Code :: ......'
        dir("/var/lib/jenkins/workspace/BlueOcean_master/java_web_code") { 
           sh 'sudo mvn install'
        }      
        echo 'Maven build complete'
      }
    }
  }
}
