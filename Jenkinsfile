pipeline {
  agent { dockerfile true }
  triggers {
    cron(env.BRANCH_NAME == 'master' ? '* * * * *' : '')
  }
  stages {
    stage("stage1") {
      steps {
        sh "./test.sh"
        echo "conditional triger for multibranch test"
      }
    }
  }
}
