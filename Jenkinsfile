pipeline {
  parameters {
    booleanParam(defaultValue: false, description: 'param1', name: 'param1')
    string(defaultValue: "deafult", description: 'param2', name: 'param2')
  }  
  agent { dockerfile true }  
  stages {
    stage("build") {
      steps {
        echo "build"
      }
    }
    stage("test") {
      steps {
        sh "./test.sh"
      }
    }
  }
}
