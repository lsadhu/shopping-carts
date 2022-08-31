pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'maven' 
    }
    

    stages{
        stage('compile-app'){
            steps{
                echo 'this is the compile-app job'
                sh 'mvm compile'
            }
        }
        stage('test-app'){
            steps{
                echo 'this is the test-app job'
                sh 'mvm test'
            }
        }
        stage('package-app'){
            steps{
                echo 'this is the package-app job'
                sh 'mvm package'
            }
        }
    }
    
    post{
        always{
            echo 'Hi, this is my first maven pipeline code completed...'
        }
        
    }
    
}
