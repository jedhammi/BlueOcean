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
    
    stage('TEST') {
      steps {
        echo "..... Test Phase Started :: Testing via Automated Scripts :: ......"
        dir("/var/lib/jenkins/workspace/BlueOcean_master/integration-testing/") { 
           sh 'mvn clean verify -P integration-test'
        }      
        echo 'Maven test complete'
      }
    }
    
  }
}
