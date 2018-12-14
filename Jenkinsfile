pipeline
{
    agent any

    stages
    {
        stage('Compile Stage')
        {
        steps{
                sh 'mvn clean compile install'
             }
        }

        stage('Testing Stage')
        {
        steps{
                sh 'mvn surefire:test -Dtest=*.java'
             }
        }

        stage('Deployment Stage')
        {
         steps{
                sh 'mvn deploy'
             }
        }

        stage('Package Stage')
        {
         steps{
                sh 'mvn package'
             }
        }

    }
}