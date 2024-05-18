pipeline{
    agent {
        docker{
            image 'node:21-alpine'
        }
    }

    
    stages{
        stage('build')
        {
           steps{
            echo 'Build applications'
            sh 'npm -v'
           }
           
        }

    
         stage('tests')
        {
            steps{
            echo 'Executions des tests '
           }
        }
          stage('dependencies')
        {
            steps{
            echo 'correction dependances'
           }
        }
         stage('deployment')
        {
            steps{
            echo 'Deploiement application'
           }
        }
    }
    post{
        always{
           echo 'always !'
        }
        success{
             echo 'success !'
        }
    }
}