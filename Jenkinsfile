pipeline{
    agent any

    
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