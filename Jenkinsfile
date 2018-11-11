pipeline {
  parameters {
    booleanParam(defaultValue: false, description: 'param1', name: 'param1')
    string(defaultValue: "deafult", description: 'param2', name: 'param2')
  }  
  agent { dockerfile true }  
  stages {
    stage("stage1") {
      steps {
        sh "./test.sh"
      }
    }
    stage("stage2") {
      steps {
        echo "test"
      }
    }
  }
}
