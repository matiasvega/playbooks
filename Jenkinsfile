pipeline {
    agent any
    environment {
        USERNAME='username' // Added variable
    }
    parameters {
        string(name: 'username', defaultValue: '', description: 'username',)
    }
    stages {
        stage(" execute Ansible") {
           steps {
					ansiblePlaybook(
					installation: 'Ansible',
                    inventory: 'inventory.ini',
					playbook: 'create_user.yml',
                    credentialsId: 'ansibleUser',
                    extraVars   : [
                        username: env.USERNAME,
                    ]
                )
            }    
        }    
    }
}
