pipeline {
	agent {
		label 'ubuntu18_jenkins_slave01'
	}
	parameters {
		string(name: 'NAME', defaultValue: 'NGUYEN KHAC MANH', description: 'This is field for the Name of you')
		text(name: 'STATE', defaultValue: 'HCM', description: 'This is field for state you live')
		choice(name: 'SEX', choices['Male', 'Female', 'Other'], description: 'choose your sex')
		booleanParam(name: 'AVAILABLE', defaultValue: true, description: 'youre available')
		password(name: 'PASSWORD', defaultValue: 'password', description: 'Enter your password')
	}
	stages {
		stage('TEST') {
			steps {
				echo 'this is the ${params.NAME}'
				echo 'this is the ${params.STATE}'
				echo 'this is the ${params.SEX}'
				echo 'this is the ${params.AVAILABLE}'
				echo 'this is the ${params.PASSWORD}'
				echo '-----------------------------'
				sh 'echo "this is name cmd ${NAME}"'
				sh 'echo -----------'
				sh 'echo "this is name cmd ${params.NAME}"'
			}
		}
	}
}