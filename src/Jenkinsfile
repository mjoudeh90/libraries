@Library('mail_list') _

pipeline{
	agent any

	stages{
		stage('buildit'){
			steps{
				script{
					mail = new emails()
					mail.mails.each { println "name: $it.key, email: $it.value" }
				}
			}
		}
	}

}
