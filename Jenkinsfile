pipeline {
    agent any
    parameters {
            string(defaultValue: "Maintainer", description: 'Enter User Role', name: 'userRole')
    }
    stages {
        stage('listVals') {
            steps {
                echo "user role = ${params.userRole}"
                post {
                    success {
                        echo "User identified"
                    }
                    failure {
                        steps {
                            echo 'Build failed'
                        }
                       
                
                    }
                    
                }
            }

        }
            

        }

    }