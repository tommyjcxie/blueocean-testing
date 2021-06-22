pipeline {
    agent any
    parameters {
		choice(name: "java_vendor", choices: "Corretto")
		choice(name: "java_version", choices: "11")
		choice(name: "browser", choices: "chrome")
	}
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
