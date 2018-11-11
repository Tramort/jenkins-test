pipeline {
  agent { dockerfile true }
  stages {
    stage("stage1") {
      steps {
        sh "./test.sh"
      }
    }
  }
}
