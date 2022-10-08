 pipeline{
    agent {label 'mvn3'}
    stages{
        stage(pull from vcs){
            steps{
                git url: 'https://github.com/Qtalha/openmrs-core.git',
                branch: 'SPRINT_1_DEV'

            }
        }
        stage{
            steps{
                sh 'mvn package' 
            }

        }
    }
 }