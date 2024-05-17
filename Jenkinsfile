pipeline{
    agent any

    stages{
        stage('build')
        {
           steps{
            echo 'Build applications'
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
}