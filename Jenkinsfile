pipeline {
    agent any  
    
    stages {
        stage('prepare env') {
            steps {
                load "${WORKSPACE}//Custom.yml"
                echo "stage 1"
            }
        }
        stage('Stage 1') {
            steps {
                echo "${DOMAIN}"
            }
        }
        stage('Stage 2') {
            steps {
                script {
                      sh 'printenv'
                }
                
            }
        }
    }
}
