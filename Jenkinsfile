pipeline {
    agent none
    stages {
        stage('Build et Test') {
            agent { label 'build' }
            steps {
                echo "Construire et tester l'application."
            }
        }
        stage('Déploiement séquentiel') {
            agent { label 'deploy' }
            stages {
                stage('Déploiement Dev') {
                    steps {
                        echo "Déploiement en environnement de développement."
                    }
                }
                stage('Déploiement Staging') {
                    steps {
                        echo "Déploiement en environnement de préproduction."
                    }
                }
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