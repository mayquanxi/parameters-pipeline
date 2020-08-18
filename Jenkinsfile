pipeline {
	agent {
		label 'ubuntu18_jenkins_slave01'
	}
	parameters {
		string(name: 'NAME', defaultValue: 'NGUYEN KHAC MANH', description: 'This is field for the Name of you')
		text(name: 'STATE', defaultValue: 'HCM', description: 'This is field for state you live')
		choice(name: 'SEX', choices: ['Male', 'Female', 'Other'], description: 'choose your sex')
		booleanParam(name: 'AVAILABLE', defaultValue: true, description: 'youre available')
		password(name: 'PASSWORD', defaultValue: 'password', description: 'Enter your password')
	}
	stages {
		stage('TEST') {
			steps {
				echo "My name: ${params.NAME}, dc: ${params.STATE}, sex: ${params.SEX}, available: ${params.AVAILABLE}, password: ${params.PASSWORD}"
				echo ""
				echo '-----------------------------'
				sh 'echo "this is name cmd ${NAME}"'
				sh 'echo "this is name cmd ${STATE}"'
				sh 'echo "this is name cmd ${SEX}"'
				sh 'echo "this is name cmd ${AVAILABLE}"'
				sh 'echo "this is name cmd ${PASSWORD}"'
				sh 'echo -----------'
			}
		}
	}
}