
pipeline {
    agent any
    stages {
        stage('Build et Test') {
            steps {
                echo "Construire et tester l'application."
            }
        }
        stage('Construction parallèle') {
            failFast true
            parallel {
                stage('test integration et dependencies') {
                    steps {
                        echo "execution tests."
                    }
                }
                stage('Déploiement Staging') {
                    steps {
                        echo "Déploiement en environnement de préproduction."
                    }
                }
            }
        }
         stage('Optimisation')
        {
            steps{
            echo 'dependencies et mise a jour des packages '
           }
        }
          stage('deploiement')
        {
            steps{
            echo 'deploiement en production'
           }
        }
         stage('montee en serveur')
        {
            steps{
            echo 'Deploiement serveur supplementaire'
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