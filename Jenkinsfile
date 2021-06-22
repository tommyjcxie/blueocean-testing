pipeline {
    agent any
    parameters {
		separator(name: "BUILD_ENVIRONMENT", sectionHeader: "Build Environment",
			separatorStyle: "border-width: 0",
			sectionHeaderStyle: """
				background-color: #7ea6d3;
				text-align: center;
				padding: 4px;
				color: #343434;
				font-size: 22px;
				font-weight: normal;
				text-transform: uppercase;
				font-family: 'Orienta', sans-serif;
				letter-spacing: 1px;
				font-style: italic;
			"""
		)
		choice(name: "java_vendor", choices: "Corretto")
		choice(name: "java_version", choices: "11")
		separator(name: "testing", sectionHeader: "Test Environment")
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
