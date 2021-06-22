pipeline {
    agent any
    parameters {
		separator(name: "BUILD_ENVIRONMENT", sectionHeader: "Build Environment"),
		choice(name: "JAVA_VENDOR", choices: ["Coretto"]),
		choice(name: "JAVA_VERSION", choices: ["11"]),
		separator(name: "TEST_ENVIRONMENT", sectionHeader: "Test Environment"),
		choice(name: "OS", choices: ["Linux"]),
		choice(name: "BROWSER", choices: ["Chrome"])
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
