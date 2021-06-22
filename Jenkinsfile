pipeline {
    agent any
    parameters {
		separator(name: "building")
		choice(name: "java_vendor", choices: "Corretto")
		choice(name: "java_version", choices: "11")
		separator(name: "testing")
		choice(name: "browser", choices: "chrome")
		separator(name: "end")
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
