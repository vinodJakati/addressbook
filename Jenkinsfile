pipeline {
    agent any

    stages {
        stage ("clone the project") {
            steps{
                git "https://github.com/upshiftnow/addressbook.git"
            }
        }
        stage ("compile") {
            steps {
                echo "executing Compilation"
                sh "mvn compile"
            }
        }
        stage ("tests") {
            steps {
                echo "executing tests"
                sh "mvn test"
            }
        }
        stage ("package") {
            steps {
                echo "Creating a package"
                sh "mvn package"
            }
        }
    }
}
