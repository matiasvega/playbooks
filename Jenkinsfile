pipeline {
    agent any
    stages {
        stage(" execute Ansible") {
           steps {
					ansiblePlaybook(
					installation: 'Ansible',
                    inventory: 'inventory.ini',
					playbook: 'test.yml'
                )
            }    
        }    
    }
}
