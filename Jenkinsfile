pipeline {
    agent any
    stages {
        stage(" execute Ansible") {
           steps {
					ansiblePlaybook(
					installation: 'Ansible',
					playbook: 'test.yml'
                )
            }    
        }    
    }
}
