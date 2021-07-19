pipeline {
  agent any
  stages {
    stage('Example') {
      input {
        message "Should we continue?"
        ok "Yes, we should."
        submitter "alice,bob"
        parameters {
          string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
        }
      }
      steps {
        echo "Hello, ${PERSON}, nice to meet you."

        script {
          buildDescription '<img src="https://himg.bdimg.com/sys/portraitn/item/31317371d0a1d3eafb58"></img>'
        }
      }
    }
  }
}