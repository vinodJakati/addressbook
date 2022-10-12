pipeline {
 
  agent any
  stages {
    stage ("clone the repository") {
      steps {
        git https://github.com/upshiftnow/addressbook.git
      }
    }
    stage ("compile the project") {
      steps {
        sh "mvn compile"
      }
    }
  }
}
