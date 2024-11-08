pipeline {
 agent any
 parameters {
    string(name: 'USER_NAME', defaultValue: 'Ajaykumar The Great', description: 'Name of the user')
    string(name: 'USER_TASK', defaultValue: 'DevOps Practical', description: 'Task of the user')
  }
 stages {
    stage('Greet User') {
        steps {
            script {
                echo "Hello, ${params.USER_NAME}! Welcome to Jenkins."
            }
        }
    }
    stage('User Task') {
        steps {
            script {
                echo "Wishing you best of luck for your ${params.USER_TASK}."
            }
        }
    }
   stage('Portfolio Website') {
        steps {
            script {
                echo "You can visit my prtfolio at https://ajaykumarn3000.github.io"
            }
        }
    }
   stage('Success') {
        steps {
            script {
                echo "DevOps Practical Executed Successfully! YAYY!!"
            }
        }
    }
 }
 post {
     always {
        echo 'Pipeline execution completed.'
     }
 }
}
